<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Katalog Komputer Sejahtera</title>
    <link rel="stylesheet" href="style4.css">
</head>
<body>

    <header>
        <h1>Katalog Komputer Sejahtera</h1>
        <p>Toko Online Laptop & Aksesoris Terpercaya</p>
    </header>

    <nav>
        <a href="#">Beranda</a>
        <a href="#">Produk</a>
        <a href="#">Promo</a>
        <a href="#">Tentang Kami</a>
        <a href="#">Kontak</a>
    </nav>

    <div class="container">
        <div class="sidebar">
            <h3>Kategori</h3>
            <ul>
                <li>Laptop</li>
                <li>Aksesoris</li>
                <li>Monitor</li>
                <li>Komponen</li>
                <li>Periferal</li>
            </ul>
        </div>

        <div class="content">
            <h2>Tentang Kami</h2>
            <p>Kami adalah toko komputer terpercaya yang menyediakan berbagai laptop, monitor, dan aksesoris komputer dengan harga bersaing. Produk kami selalu up-to-date dan bergaransi resmi.</p>
            <p>Belanja mudah, aman, dan cepat hanya di Komputer Sejahtera — solusi lengkap untuk kebutuhan teknologi Anda.</p>
        </div>
    </div>

    <div class="container">
        <div class="content">
            <h2>Katalog Produk Terbaru</h2>
            <div class="catalog-container">
                <div class="product-card">
                    <img src="https://share.google/images/s8YpXcU6Xgu4YCeXS" alt="Laptop Gaming">
                    <h3>Laptop Gaming</h3>
                    <p class="price">Rp 14.500.000</p>
                    <button>Detail</button>
                </div>

                <div class="product-card">
                    <img src="https://images.unsplash.com/photo-1587202372775-bd07f61f8a58" alt="Mouse Wireless">
                    <h3>Mouse Wireless</h3>
                    <p class="price">Rp 250.000</p>
                    <button>Detail</button>
                </div>

                <div class="product-card">
                    <img src="https://images.unsplash.com/photo-1587202372775-9890d6a5dc57" alt="Keyboard Mechanical">
                    <h3>Keyboard Mechanical</h3>
                    <p class="price">Rp 850.000</p>
                    <button>Detail</button>
                </div>

                <div class="product-card">
                    <img src="https://share.google/images/r1v9yOBS2WIB8itIL" alt="Monitor 24 inch">
                    <h3>Monitor 24 Inch</h3>
                    <p class="price">Rp 2.750.000</p>
                    <button>Detail</button>
                </div>

                <div class="product-card">
                    <img src="https://share.google/images/DEmwaobptO60iA5OF" alt="Headset Gaming">
                    <h3>Headset Gaming</h3>
                    <p class="price">Rp 490.000</p>
                    <button>Detail</button>
                </div>

                <div class="product-card">
                    <img src="https://share.google/images/xTnpQVnMQenmOHCTz" alt="Webcam HD">
                    <h3>Webcam HD</h3>
                    <p class="price">Rp 399.000</p>
                    <button>Detail</button>
                </div>
            </div>
        </div>
    </div>

    <footer>
        &copy; 2025 Komputer Sejahtera. Semua Hak Dilindungi.
    </footer>

</body>
</html>

CSS
/* === Gaya Umum === */
body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  margin: 0;
  background-color: #f0f2f5;
}

/* === Header === */
header {
  background-color: #237dad;
  color: white;
  padding: 25px;
  text-align: center;
  position: sticky;
  top: 0;
  z-index: 1000;
  box-shadow: 0 2px 6px rgba(0,0,0,0.2);
}

header h1 {
  margin: 0;
  font-size: 28px;
}

header p {
  margin: 5px 0 0;
  font-size: 16px;
}

/* === Navigasi === */
nav {
  background-color: #125d8a;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  padding: 10px;
  position: sticky;
  top: 80px;
  z-index: 999;
}

nav a {
  color: white;
  text-decoration: none;
  padding: 10px 20px;
  margin: 5px;
  background-color: #1f78b4;
  border-radius: 5px;
  transition: all 0.3s ease;
  font-weight: 500;
}

nav a:hover {
  background-color: #0b4f70;
  transform: scale(1.05);
}

/* === Layout Utama === */
.container {
  display: flex;
  gap: 20px;
  padding: 20px;
}

/* === Sidebar === */
.sidebar {
  flex: 1;
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 5px rgba(0,0,0,0.2);
  height: fit-content;
}

.sidebar h2 {
  margin-top: 0;
  color: #125d8a;
}

.sidebar ul {
  list-style: none;
  padding-left: 0;
}

.sidebar ul li {
  padding: 8px 0;
  border-bottom: 1px solid #ddd;
  color: #333;
  cursor: pointer;
  transition: color 0.3s;
}

.sidebar ul li:hover {
  color: #125d8a;
}

/* === Konten Produk === */
.content {
  flex: 3;
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 5px rgba(0,0,0,0.2);
}

.content h2 {
  color: #125d8a;
  border-bottom: 2px solid #125d8a;
  padding-bottom: 10px;
}

/* === Katalog Produk === */
.catalog-container {
  display: flex;
  flex-wrap: nowrap;
  overflow-x: auto;
  gap: 20px;
  padding: 20px 0;
  scroll-snap-type: x mandatory;
}

/* Scroll bar tipis */
.catalog-container::-webkit-scrollbar {
  height: 8px;
}
.catalog-container::-webkit-scrollbar-thumb {
  background-color: #ccc;
  border-radius: 10px;
}

.product-card {
  flex: 0 0 auto;
  width: 250px;
  background-color: white;
  border-radius: 15px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
  transition: transform 0.3s, box-shadow 0.3s;
  scroll-snap-align: start;
  text-align: center;
  overflow: hidden;
}

.product-card img {
  width: 100%;
  height: 160px;
  object-fit: cover;
  border-radius: 15px 15px 0 0;
}

.product-card h3 {
  margin: 15px 0 5px;
  color: #333;
  font-size: 18px;
}

.product-card .price {
  color: #008cba;
  font-weight: bold;
  margin-bottom: 10px;
  font-size: 16px;
}

.product-card button {
  background-color: #008cba;
  border: none;
  color: white;
  padding: 10px 15px;
  border-radius: 8px;
  cursor: pointer;
  transition: background 0.3s, transform 0.2s;
  margin-bottom: 15px;
}

.product-card button:hover {
  background-color: #005f7f;
  transform: scale(1.05);
}

.product-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 8px 18px rgba(0,0,0,0.2);
}

/* === Footer === */
footer {
  background-color: #237dad;
  color: white;
  text-align: center;
  padding: 15px;
  margin-top: 20px;
  box-shadow: 0 -2px 5px rgba(0,0,0,0.1);
}

/* === Responsif === */
@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }

  nav {
    position: static;
  }

  .product-card {
    width: 80%;
    margin: 0 auto;
  }
}
