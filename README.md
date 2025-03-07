<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A to Zee Hearing Solutions</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; margin: 0; padding: 0; background: #e0f2f1; color: black; overflow-x: hidden; }
        .header { background: #004d40; color: white; padding: 20px; font-size: 24px; animation: fadeInDown 1s ease-in-out; }
        .navbar { display: flex; justify-content: center; background: #00332a; padding: 10px; }
        .navbar a { color: white; text-decoration: none; padding: 10px 15px; transition: color 0.3s; }
        .navbar a:hover { color: #e0f2f1; }
        .hero { background: url('https://via.placeholder.com/1200x400') center/cover no-repeat; padding: 50px; color: white; font-size: 32px; font-weight: bold; animation: fadeIn 2s ease-in-out; }
        .section { padding: 20px; transition: transform 0.3s ease-in-out, opacity 0.5s ease-in-out; opacity: 0; transform: translateY(20px); }
        .section.visible { opacity: 1; transform: translateY(0); }
        .btn { background: #004d40; color: white; padding: 10px 20px; border: none; cursor: pointer; text-decoration: none; transition: background 0.3s, transform 0.2s; }
        .btn:hover { background: #00251a; transform: scale(1.05); }
        .footer { background: black; color: white; padding: 10px; text-align: center; }
        .image-container { display: flex; flex-wrap: wrap; justify-content: center; gap: 10px; padding: 20px; }
        .image-container img { width: 200px; height: auto; border-radius: 10px; transition: transform 0.3s, box-shadow 0.3s; }
        .image-container img:hover { transform: scale(1.1); box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.3); }
        @keyframes fadeInDown { from { opacity: 0; transform: translateY(-20px); } to { opacity: 1; transform: translateY(0); } }
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
    </style>
</head>
<body>
    <div class="header">Welcome to A to Zee Hearing Solutions</div>
    <div class="navbar">
        <a href="#about">About Us</a>
        <a href="#services">Services</a>
        <a href="#products">Products</a>
        <a href="#contact">Contact</a>
    </div>
    <div class="hero">Your Trusted Hearing Aid Partner</div>
    
    <div class="section" id="about">
        <h2>About Us</h2>
        <p>A to Zee Hearing Solutions is a trusted hearing aids consultant and wholesaler, providing expert solutions for better hearing.</p>
    </div>
    
    <div class="section" id="services">
        <h2>Our Services</h2>
        <p>We offer hearing tests, consultation, hearing aid fittings, and high-quality hearing aids at wholesale prices.</p>
    </div>
    
    <div class="section" id="products">
        <h2>Our Products</h2>
        <div class="image-container">
            <img src="https://via.placeholder.com/200" alt="Hearing Aid 1">
            <img src="https://via.placeholder.com/200" alt="Hearing Aid 2">
            <img src="https://via.placeholder.com/200" alt="Hearing Aid 3">
            <img src="https://via.placeholder.com/200" alt="Hearing Aid 4">
        </div>
    </div>
    
    <div class="section" id="contact">
        <h2>Contact Us</h2>
        <p>📍 Address: B-1300, 4th B Road, Kali Tanki, Satellite Town, Rawalpindi</p>
        <p>📞 Phone: 03335155473</p>
        <a href="tel:03335155473" class="btn">Call Now</a>
        <h3>Find Us on Google Maps</h3>
        <iframe 
            width="600" 
            height="450" 
            style="border:0" 
            loading="lazy" 
            allowfullscreen 
            referrerpolicy="no-referrer-when-downgrade"
            src="https://www.google.com/maps/embed/v1/place?key=YOUR_GOOGLE_MAPS_API_KEY&q=B-1300,4th+B+Road,Kali+Tanki,Satellite+Town,Rawalpindi">
        </iframe>
    </div>
    
    <div class="footer">&copy; 2025 A to Zee Hearing Solutions | All Rights Reserved</div>
    
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            const sections = document.querySelectorAll(".section");
            function revealOnScroll() {
                sections.forEach(section => {
                    const sectionTop = section.getBoundingClientRect().top;
                    if (sectionTop < window.innerHeight - 100) {
                        section.classList.add("visible");
                    }
                });
            }
            window.addEventListener("scroll", revealOnScroll);
            revealOnScroll();
        });
    </script>
</body>
</html>
