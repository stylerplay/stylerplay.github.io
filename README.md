<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Portofolio Saya</title>

  <!-- Bootstrap 5 -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
  
  <!-- AOS Animation -->
  <link href="https://unpkg.com/aos@2.3.4/dist/aos.css" rel="stylesheet">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.5/font/bootstrap-icons.css" rel="stylesheet">
  
  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">

  <style>
    body {
      font-family: 'Poppins', sans-serif;
      transition: background 0.3s, color 0.3s;
    }

    header {
      background: linear-gradient(to right, #0f2027, #203a43, #2c5364);
      color: white;
      padding: 4rem 0 6rem;
      text-align: center;
    }

    header img {
      object-fitcocoverocover;

      box-shadowadowadowadowadowadowadaaadowadowadowadowadowadowadaadowadowadowadowadowadowadadowadowadowadowadowadowadowadow: 0 4px 10px rgba(0,0,0,0.3);
      animation: float 3s ease-in-out infinite;
    }

    @keyframes float {
      0%   { transform: translateY(0px); }
      50%  { transform: translateY(-10px); }
      100% { transform: translateY(0px); }
    }

    section {
      padding: 60px 0;
    }

    .navbar {
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }

    .skills li {
      display: inline-block;
      background: #e3f2fd;
      color: #0d47a1;
      padding: 8px 16px;
      margin: 6px;
      border-radius: 25px;
      font-weight: 500;
    }

    .project-card {
      border: 1px solid #ddd;
      border-radius: 10px;
      padding: 20px;
      background: white;
      transition: transform 0.3s;
    }

    .project-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }

    footer {
      background: #203a43;
      color: white;
      text-align: center;
      padding: 20px 0;
    }

    /* Dark mode support */
    @media (prefers-color-scheme: dark) {
      body {
        background: #121212;
        color: #eee;
      }

      .skills li {
        background: #263238;
        color: #90caf9;
      }

      .project-card {
        background: #1e1e1e;
        border-color: #333;
      }

      .form-control {
        background: #1e1e1e;
        color: #fff;
        border-color: #444;
      }

      .form-control::placeholder {
        color: #aaa;
      }

      .btn-primary {
        background-color: #0d47a1;
        border-color: #0d47a1;
      }

      footer {
        background: #0d0d0d;
      }
    }
  </style>
</head>
<body>

<!-- Navbar -->
<nav class="navbar navbar-expand-lg navbar-light bg-light sticky-top">
  <div class="container">
    <a class="navbar-brand fw-bold" href="#">Portofolio</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navmenu">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navmenu">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item"><a href="#about" class="nav-link">Tentang</a></li>
        <li class="nav-item"><a href="#skills" class="nav-link">Keahlian</a></li>
        <li class="nav-item"><a href="#projects" class="nav-link">Proyek</a></li>
        <li class="nav-item"><a href="#contact" class="nav-link">Kontak</a></li>
      </ul>
    </div>
  </div>
</nav>

<!-- Hero -->
<header>
  <div class="container">
    <img src="profil.jpg" alt="Foto Profil" data-aos="zoom-in">
    <h1 data-aos="fade-down" class="mt-3">Nijar Padilah</h1>
    <p class="lead" data-aos="fade-up" data-aos-delay="200">Web Developer Pemula </p>
  </div>
</header>

<!-- Tentang -->
<section id="about">
  <div class="container" data-aos="fade-up">
    <h2 class="text-center mb-4">Tentang Saya</h2>
    <p class="text-center">Saya adalah seorang web developer yang fokus pada pembuatan website modern, responsif, dan cepat. Saya senang mengeksplorasi teknologi dan berkontribusi dalam proyek-proyek yang berdampak nyata.</p>
  </div>
</section>

<!-- Keahlian -->
<section id="skills" class="bg-light">
  <div class="container" data-aos="fade-up">
    <h2 class="text-center mb-4">Keahlian</h2>
    <ul class="skills text-center list-unstyled">
      <li>HTML</li>
      <li>CSS</li>
      <li>PHP</li>
      <li>Laravel</li>
    </ul>
  </div>
</section>

<!-- Proyek -->
<section id="projects">
  <div class="container" data-aos="fade-up">
    <h2 class="text-center mb-4">Proyek</h2>
    <div class="row g-4">
      <div class="col-md-6">
        <div class="project-card">
          <h5>Website Toko Online</h5>
          <p>Membangun toko online dengan fitur lengkap: keranjang, pembayaran, dan dashboard admin berbasis Laravel.</p>
        </div>
      </div>
      <div class="col-md-6">
        <div class="project-card">
          <h5>Landing Page Produk</h5>
          <p>Desain responsif untuk halaman promosi produk digital yang mengoptimalkan konversi pengguna.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Kontak -->
<section id="contact" class="bg-light">
  <div class="container" data-aos="fade-up">
    <h2 class="text-center mb-4">Kontak Saya</h2>
    <form class="mx-auto" style="max-width: 600px;">
      <div class="mb-3">
        <input type="text" class="form-control" placeholder="Nama Anda" required>
      </div>
      <div class="mb-3">
        <input type="email" class="form-control" placeholder="Email Anda" required>
      </div>
      <div class="mb-3">
        <textarea class="form-control" rows="5" placeholder="Pesan Anda" required></textarea>
      </div>
      <div class="d-grid">
        <button type="submit" class="btn btn-primary">Kirim Pesan</button>
      </div>
    </form>
  </div>
</section>

<!-- Sosial Media -->
<section class="text-center py-4" data-aos="fade-up">
  <h2 class="mb-3">Ikuti Saya</h2>
  <div class="d-flex justify-content-center gap-4 fs-3">
    <a href="https://wa.me/+6281213966455" class="text-success" target="_blank" title="WhatsApp">
      <i class="bi bi-whatsapp"></i>
    </a>
    <a href="https://www.instagram.com/204k_np?igsh=NXhrcTFuZTk4ZHE1" class="text-danger" target="_blank" title="Instagram">
      <i class="bi bi-instagram"></i>
    </a>
    <a href="https://github.com/nama_kamu" class="text-dark" target="_blank" title="GitHub">
      <i class="bi bi-github"></i>
    </a>
    <a href="https://www.linkedin.com/in/nijar-padillah-872a43372" class="text-primary" target="_blank" title="LinkedIn">
      <i class="bi bi-linkedin"></i>
    </a>
  </div>
</section>


<!-- Footer -->
<footer>
  <div class="container">
    <p>&copy; 2025 Semua hak dilindungi.</p>
  </div>
</footer>

<!-- Scripts -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
<script src="https://unpkg.com/aos@2.3.4/dist/aos.js"></script>
<script>
  AOS.init();
</script>

</body>
</html>
