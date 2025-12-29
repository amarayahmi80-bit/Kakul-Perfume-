// Smooth scrolling for navigation links
document.querySelectorAll('nav a').forEach(anchor => {
    anchor.addEventListener('click', function(e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        target.scrollIntoView({ behavior: 'smooth' });
    });
});

// Simple add to cart alert
document.querySelectorAll('.product-card button').forEach(button => {
    button.addEventListener('click', () => {
        alert('Added to cart! (Demo - integrate with e-commerce like Shopify for Kakul Perfume.)');
    });
});

// Form submission (demo)
document.querySelector('.contact form').addEventListener('submit', function(e) {
    e.preventDefault();
    alert('Thank you for reaching out to Kakul Perfume! We\'ll respond soon.');
});
