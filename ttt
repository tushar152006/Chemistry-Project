function plotSpectrum() {
    const wavelength = document.getElementById("wavelength-input").value;
    const ctx = document.getElementById("spectrumChart").getContext('2d');

    const spectrumData = {
        labels: ['Ultraviolet', 'Visible', 'Infrared'],
        datasets: [{
            label: 'Absorption Spectrum',
            data: [100 - wavelength, wavelength - 300, wavelength - 600],
            backgroundColor: ['rgba(0, 123, 255, 0.5)', 'rgba(255, 99, 132, 0.5)', 'rgba(75, 192, 192, 0.5)']
        }]
    };

    new Chart(ctx, {
        type: 'bar',
        data: spectrumData,
        options: {
            scales: {
                y: {
                    beginAtZero: true
                }
            }
        }
    });
}
