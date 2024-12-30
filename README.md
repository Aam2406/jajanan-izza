# <!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website Makanan Bergerak</title>
    <style>
        /* Reset margin dan padding */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Body Styles */
body {
    font-family: 'Arial', sans-serif;
    background-color: #f4f4f4;
    color: #333;
    overflow-x: hidden; /* Menghindari scroll horizontal */
}

/* Header Styles */
.header {
    background-color: #ff6347;
    color: white;
    padding: 40px 20px;
    text-align: center;
    animation: fadeIn 1s ease-out;
}

.header h1 {
    font-size: 36px;
    margin-bottom: 10px;
}

.header p {
    font-size: 18px;
}

/* Menu Section */
.menu {
    display: flex;
    justify-content: space-around;
    margin: 50px 0;
    animation: slideUp 1.5s ease-out;
}

.menu-item {
    background-color: white;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
    width: 30%;
    margin: 20px;
    padding: 15px;
    transition: transform 0.3s ease;
    animation: fadeInItem 1.5s ease-out;
}

.menu-item:hover {
    transform: translateY(-10px);
}

.food-image {
    width: 100%;
    height: auto;
    border-radius: 8px;
    transition: transform 0.3s ease-in-out;
}

.food-image:hover {
    transform: scale(1.1); /* Efek zoom pada gambar */
}

.menu-item h3 {
    font-size: 22px;
    margin-top: 15px;
}

button.order-btn {
    background-color: #ff6347;
    color: white;
    border: none;
    padding: 12px 20px;
    font-size: 16px;
    border-radius: 5px;
    cursor: pointer;
    margin-top: 15px;
    transition: background-color 0.3s ease;
}

button.order-btn:hover {
    background-color: #e55347;
}

/* Footer Styles */
footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 20px;
    animation: fadeIn 2s ease-out;
}

footer p {
    font-size: 16px;
}

footer strong {
    color: #ff6347;
}

/* Animasi untuk elemen yang masuk */
@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* Animasi untuk menu item */
@keyframes fadeInItem {
    from {
        opacity: 0;
        transform: scale(0.8);
    }
    to {
        opacity: 1;
        transform: scale(1);
    }
}

/* Animasi untuk menu section */
@keyframes slideUp {
    from {
        opacity: 0;
        transform: translateY(50px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* Responsive Design */
@media (max-width: 768px) {
    .menu {
        flex-direction: column;
        align-items: center;
    }

    .menu-item {
        width: 80%;
    }
}

@media (max-width: 480px) {
    .menu-item {
        width: 90%;
    }

    .header h1 {
        font-size: 28px;
    }

    .header p {
        font-size: 16px;
    }
}

button.order-btn a {
    color: white;
    text-decoration: none;
    display: block;
    width: 100%;
    height: 100%;
    padding: 12px 20px;
}

button.order-btn:hover {
    background-color: #e55347;
}

    </style>
<body>
    <!-- Header -->
    <header class="header">
        <h1>Selamat Datang di IZZA FOOD!</h1>
        <p>Temukan menu favoritmu dan rasakan sensasi baru!</p>
    </header>

    <!-- Menu Section -->
    <section class="menu">
        <div class="menu-item">
            <img src="cuanki.jpg" alt="Odeng KW" class="food-image">
            <h3>Odeng KW</h3>
           <p>terbuat dari blablablabla</p>
           <h3>Harga: 10k/Bungkus</h3>
           <h4  style="background-color: #e55347;"><strong>Ready</strong></h4>
        </div>
        <div class="menu-item">
            <img src="bakso.jpg" alt="Burger" class="food-image">
            <h3>Cilok Balado</h3>
            <p>terbuat dari blablablabla</p>
            <h3>Harga: 10k/Bungkus</h3>
            <h4  style="background-color: #e55347;"><strong>Sold Out</strong></h4>
        </div>
        <div class="menu-item">
            <img src="kerupuk.jpg" alt="Odeng Ikan" class="food-image">
            <h3>Odeng Ikan</h3>
            <p>terbuat dari blablablabla</p>
           <h3>Harga: 12k/Bungkus</h3>
           <h4  style="background-color: #e55347;"><strong>Sold Out</strong></h4>
        </div>
        <div class="menu-item">
            <img src="mieee.jpg" alt="Indomie Perang" class="food-image">
            <h3>IndomiePerang</h3>
            <p>terbuat dari blablablabla</p>
           <h3>Harga: 10k/Bungkus</h3>
           <h4  style="background-color: #e55347;"><strong>Ready</strong></h4>
        </div>
        <div class="menu-item">
            <img src="miegg.jpg" alt="Mie GG" class="food-image">
            <h3>Mie GG</h3>
            <p>terbuat dari blablablabla</p>
           <h3>Harga: 10k/Bungkus</h3>
           <h4  style="background-color: #e55347;"><strong>Ready</strong></h4>
        </div>
        <div class="menu-item">
            <img src="risol.jpg" alt="Roti Isi" class="food-image">
            <h3>Roti Isi</h3>
            <p>terbuat dari blablablabla</p>
           <h3>Harga: <br>7,5/satuan</h3>
           <h4  style="background-color: #e55347;"><strong>Sold Out</strong></h4>
        </div>
        <div class="menu-item">
            <img src="sempol.jpg" alt="sempol" class="food-image">
            <h3>sempol</h3>
            <p>terbuat dari blablablabla</p>
           <h3>Harga: 10k/Bungkus</h3>
           <h4 style="background-color: #e55347;"><strong>Ready</strong></h4>
        </div>
        
    </section>

    <!-- Footer -->
    <footer>
        <p>Hubungi kami di: <strong>+62 812-3456-7890</strong></p>
        <p>&copy; 2024 IZZA FOOD</p>
    </footer>

<p align="center">
    <button class="order-btn">
        <a href="https://wa.me/+6281371953082" target="_blank">
            Pesan Lewat WhatsApp
        </a>
    </button>
</p>
    <script>
        // Event listener untuk tombol pesan
const orderButtons = document.querySelectorAll('.order-btn');
orderButtons.forEach(button => {
    button.addEventListener('click', function() {
        alert('Pesanan Anda telah diterima! Terima kasih.');
    });
});


    </script>
</body>
</html>
za
web
