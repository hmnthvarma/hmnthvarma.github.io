document.addEventListener('DOMContentLoaded', () => {
    const locations = document.querySelectorAll('.location');
    const tooltip = document.querySelector('.tooltip');

    if (!tooltip) {
        console.error('Tooltip element not found!');
        return;
    }

    locations.forEach(location => {
        location.addEventListener('mouseenter', (e) => {
            const place = location.getAttribute('data-place');
            const year = location.getAttribute('data-year');
            const img = location.getAttribute('data-img');
            tooltip.innerHTML = `<strong>${place}</strong><br>Visited: ${year}<br><img src="${img}" alt="${place}" onerror="this.style.display='none'">`;
            tooltip.style.display = 'block';
            tooltip.style.left = `${e.pageX + 10}px`;
            tooltip.style.top = `${e.pageY + 10}px`;
        });

        location.addEventListener('mousemove', (e) => {
            tooltip.style.left = `${e.pageX + 10}px`;
            tooltip.style.top = `${e.pageY + 10}px`;
        });

        location.addEventListener('mouseleave', () => {
            tooltip.style.display = 'none';
        });
    });
});
