<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Complete Business Landing Page</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <style>
         :root {
            --primary-color: #333;
            --secondary-color: #666;
        }
        
        body {
            font-family: Arial, sans-serif;
        }
        
        .navbar-brand {
            font-weight: bold;
            font-size: 1.5rem;
        }
        
        .hero-section {
            background-color: #f8f9fa;
            padding: 100px 0;
            text-align: center;
        }
        
        .hero-title {
            font-size: 2.5rem;
            font-weight: bold;
            margin-bottom: 20px;
        }
        
        .hero-subtitle {
            font-size: 1.5rem;
            color: var(--secondary-color);
            margin-bottom: 30px;
        }
        
        .carousel-indicators {
            bottom: -50px;
        }
        
        .carousel-indicators button {
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background-color: #ccc;
        }
        
        .carousel-indicators .active {
            background-color: var(--primary-color);
        }
        
        .section {
            padding: 80px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 20px;
            font-weight: bold;
        }
        
        .section-subtitle {
            text-align: center;
            color: var(--secondary-color);
            margin-bottom: 50px;
        }
        
        .service-card {
            text-align: center;
            margin-bottom: 30px;
        }
        
        .service-icon {
            font-size: 2rem;
            margin-bottom: 20px;
        }
        
        .service-title {
            font-weight: bold;
            margin-bottom: 15px;
        }
        
        .service-description {
            color: var(--secondary-color);
        }
        
        .why-choose-us {
            background-color: #f8f9fa;
        }
        
        .feature-box {
            display: flex;
            align-items: start;
            margin-bottom: 30px;
        }
        
        .feature-icon {
            background-color: #e9ecef;
            padding: 15px;
            border-radius: 10px;
            margin-right: 20px;
            flex-shrink: 0;
        }
        
        .feature-icon i {
            font-size: 24px;
            color: #333;
        }
        
        .feature-content h4 {
            font-size: 18px;
            margin-bottom: 10px;
            font-weight: bold;
        }
        
        .feature-content p {
            color: var(--secondary-color);
            margin-bottom: 0;
        }
        
        .image-placeholder {
            background-color: #e9ecef;
            height: 100%;
            min-height: 400px;
            border-radius: 10px;
        }
        /* Parallax Section Styles */
        
        .parallax-section {
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('/api/placeholder/1920/1080');
            background-attachment: fixed;
            background-position: center;
            background-repeat: no-repeat;
            background-size: cover;
            padding: 100px 0;
            text-align: center;
            color: white;
        }
        
        .parallax-title {
            font-size: 2.5rem;
            font-weight: bold;
            margin-bottom: 20px;
        }
        
        .parallax-subtitle {
            font-size: 1.2rem;
            margin-bottom: 30px;
        }
        
        .btn-contact {
            background-color: #666;
            color: white;
            padding: 12px 35px;
            border: none;
            border-radius: 5px;
            font-size: 1.1rem;
            transition: background-color 0.3s;
            display: inline-flex;
            align-items: center;
            justify-content: center;
        }
        
        .btn-contact i {
            margin-right: 10px;
        }
        
        .btn-contact:hover {
            background-color: #555;
            color: white;
        }
        /* Products Section Styles */
        
        .products-section {
            padding: 80px 0;
            background-color: #ffffff;
        }
        
        .products-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 40px;
        }
        
        .search-box {
            padding: 10px 20px;
            border: 1px solid #ddd;
            border-radius: 5px;
            width: 250px;
        }
        
        .product-grid {
            display: grid;
            grid-template-columns: repeat(6, 1fr);
            gap: 20px;
        }
        
        .product-card {
            background-color: #f8f9fa;
            border-radius: 10px;
            padding: 15px;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s;
        }
        
        .product-card:hover {
            transform: translateY(-5px);
        }
        
        .product-image {
            background-color: #e9ecef;
            height: 150px;
            border-radius: 5px;
            margin-bottom: 15px;
        }
        
        .product-title {
            font-weight: 600;
            font-size: 0.9rem;
            margin-bottom: 10px;
            color: #333;
        }
        
        .product-price {
            color: #333;
            font-weight: bold;
            font-size: 1rem;
        }
        
        @media (max-width: 1200px) {
            .product-grid {
                grid-template-columns: repeat(4, 1fr);
            }
        }
        
        @media (max-width: 768px) {
            .product-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            .products-header {
                flex-direction: column;
                gap: 20px;
            }
            .search-box {
                width: 100%;
            }
        }
    </style>
</head>

<body>
    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <div class="container">
            <a class="navbar-brand" href="#">BrandName</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="#">Beranda</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Tentang Kami</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Layanan</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Belanja</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Artikel</a>
                    </li>
                    <li class="nav-item">
                        <a class="btn btn-primary" href="#">Daftar Sekarang</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero-section">
        <div class="container">
            <div id="heroCarousel" class="carousel slide" data-bs-ride="carousel">
                <div class="carousel-inner">
                    <div class="carousel-item active">
                        <h1 class="hero-title">Tingkatkan Produktivitas Bisnis Anda<br>dengan [Nama Produk/Layanan].</h1>
                        <p class="hero-subtitle">Solusi Cepat dan Efisien!</p>
                    </div>
                    <div class="carousel-item">
                        <h1 class="hero-title">Solusi Bisnis Terpercaya<br>untuk Kesuksesan Anda</h1>
                        <p class="hero-subtitle">Tingkatkan Efisiensi Operasional!</p>
                    </div>
                </div>
                <div class="carousel-indicators">
                    <button type="button" data-bs-target="#heroCarousel" data-bs-slide-to="0" class="active"></button>
                    <button type="button" data-bs-target="#heroCarousel" data-bs-slide-to="1"></button>
                    <button type="button" data-bs-target="#heroCarousel" data-bs-slide-to="2"></button>
                    <button type="button" data-bs-target="#heroCarousel" data-bs-slide-to="3"></button>
                    <button type="button" data-bs-target="#heroCarousel" data-bs-slide-to="4"></button>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="section">
        <div class="container">
            <h2 class="section-title">Hal Yang Kami Tawarkan</h2>
            <p class="section-subtitle">Kami Hadir dengan Produk dan Layanan Berkualitas<br>yang Siap Menjawab Tantangan Anda.</p>

            <div class="row">
                <div class="col-md-4">
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-comments"></i>
                        </div>
                        <h3 class="service-title">Konsultasi Profesional</h3>
                        <p class="service-description">Kami menawarkan layanan konsultasi untuk membantu Anda menemukan solusi terbaik yang sesuai dengan kebutuhan spesifik bisnis Anda.</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-chart-line"></i>
                        </div>
                        <h3 class="service-title">Konsultasi Profesional</h3>
                        <p class="service-description">Kami menawarkan layanan konsultasi untuk membantu Anda menemukan solusi terbaik yang sesuai dengan kebutuhan spesifik bisnis Anda.</p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="service-card">
                        <div class="service-icon">
                            <i class="fas fa-cog"></i>
                        </div>
                        <h3 class="service-title">Konsultasi Profesional</h3>
                        <p class="service-description">Kami menawarkan layanan konsultasi untuk membantu Anda menemukan solusi terbaik yang sesuai dengan kebutuhan spesifik bisnis Anda.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Why Choose Us Section -->
    <section class="section why-choose-us">
        <div class="container">
            <div class="row">
                <div class="col-lg-6">
                    <div class="image-placeholder"></div>
                </div>
                <div class="col-lg-6">
                    <h2 class="section-title">Kenapa Anda Harus Pilih Kami?</h2>
                    <p class="section-subtitle">Karena Kami Memberikan Solusi yang Teruji dengan Kualitas Terbaik dan Layanan Terpercaya.</p>

                    <div class="feature-box">
                        <div class="feature-icon">
                            <i class="fas fa-cube"></i>
                        </div>
                        <div class="feature-content">
                            <h4>Pengalaman yang Teruji</h4>
                            <p>Kami telah membangun reputasi solid melalui pengalaman dan kerja keras, menjadikan kami mitra terpercaya dalam industri ini.</p>
                        </div>
                    </div>

                    <div class="feature-box">
                        <div class="feature-icon">
                            <i class="fas fa-cube"></i>
                        </div>
                        <div class="feature-content">
                            <h4>Pengalaman yang Teruji</h4>
                            <p>Kami telah membangun reputasi solid melalui pengalaman dan kerja keras, menjadikan kami mitra terpercaya dalam industri ini.</p>
                        </div>
                    </div>

                    <div class="feature-box">
                        <div class="feature-icon">
                            <i class="fas fa-cube"></i>
                        </div>
                        <div class="feature-content">
                            <h4>Pengalaman yang Teruji</h4>
                            <p>Kami telah membangun reputasi solid melalui pengalaman dan kerja keras, menjadikan kami mitra terpercaya dalam industri ini.</p>
                        </div>
                    </div>

                    <div class="feature-box">
                        <div class="feature-icon">
                            <i class="fas fa-cube"></i>
                        </div>
                        <div class="feature-content">
                            <h4>Pengalaman yang Teruji</h4>
                            <p>Kami telah membangun reputasi solid melalui pengalaman dan kerja keras, menjadikan kami mitra terpercaya dalam industri ini.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Parallax Section -->
    <section class="parallax-section">
