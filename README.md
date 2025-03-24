<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sport Car Collection</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Sport Car Collection</h1>
        <nav>
            <ul>
                <li><a href="#cars">Cars</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="cars" class="car-list">
        <div class="car-item">
            <img src="https://upload.wikimedia.org/wikipedia/commons/9/96/2020_Ferrari_F8_Tributo_%28D98%29_V8_%28crop%29.jpg" alt="Ferrari F8 Tributo" class="car-image">
            <h3>Ferrari F8 Tributo</h3>
            <p>The Ferrari F8 Tributo is a powerful, beautiful sports car with a 710 horsepower engine and breathtaking acceleration.</p>
            <button class="more-info-btn">Learn More</button>
        </div>
        <div class="car-item">
            <img src="https://upload.wikimedia.org/wikipedia/commons/2/25/2012_Lamborghini_Aventador_SLP_5000.jpg" alt="Lamborghini Aventador" class="car-image">
            <h3>Lamborghini Aventador</h3>
            <p>With a stunning V12 engine, the Lamborghini Aventador is designed for ultimate performance and extreme style.</p>
            <button class="more-info-btn">Learn More</button>
        </div>
        <div class="car-item">
            <img src="https://upload.wikimedia.org/wikipedia/commons/1/1f/2020_Porsche_911_Turbo_S_Coupe_%28Wikimedia%29.jpg" alt="Porsche 911 Turbo" class="car-image">
            <h3>Porsche 911 Turbo</h3>
            <p>The Porsche 911 Turbo combines speed, elegance, and timeless design, making it a top contender in the sports car world.</p>
            <button class="more-info-btn">Learn More</button>
        </div>
        <div class="car-item">
            <img src="https://upload.wikimedia.org/wikipedia/commons/f/fd/McLaren_720S_Coupe.jpg" alt="McLaren 720S" class="car-image">
            <h3>McLaren 720S</h3>
            <p>With its sleek aerodynamics and 710 horsepower engine, the McLaren 720S is a high-performance masterpiece.</p>
            <button class="more-info-btn">Learn More</button>
        </div>
    </section>

    <footer id="contact">
        <p>&copy; 2025 Sport Car Collection</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f8f8f8;
    color: #333;
}

header {
    background-color: #222;
    color: white;
    padding: 20px;
    text-align: center;
}

header h1 {
    font-size: 2.5em;
    margin-bottom: 10px;
}

nav ul {
    list-style-type: none;
}

nav ul li {
    display: inline;
    margin-right: 15px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
    font-weight: bold;
}

.car-list {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
    padding: 50px 20px;
}

.car-item {
    background-color: #fff;
    border-radius: 10px;
    width: 300px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    overflow: hidden;
    text-align: center;
}

.car-image {
    width: 100%;
    height: auto;
    transition: transform 0.3s ease-in-out;
}

.car-image:hover {
    transform: scale(1.05);
}

.car-item h3 {
    font-size: 1.8em;
    margin-top: 10px;
    color: #333;
}

.car-item p {
    padding: 10px;
    font-size: 1em;
    color: #666;
}

button.more-info-btn {
    background-color: #ff5733;
    color: white;
    border: none;
    padding: 12px 25px;
    font-size: 16px;
    cursor: pointer;
    margin-top: 20px;
    border-radius: 5px;
    transition: background-color 0.3s ease;
}

button.more-info-btn:hover {
    background-color: #ff2a00;
}

footer {
    background-color: #222;
    color: white;
    text-align: center;
    padding: 10px;
    position: fixed;
    width: 100%;
    bottom: 0;
}
// Add an event listener to all "Learn More" buttons
document.querySelectorAll('.more-info-btn').forEach(button => {
    button.addEventListener('click', () => {
        alert('More information about this amazing sports car will be available soon!');
    });
});
