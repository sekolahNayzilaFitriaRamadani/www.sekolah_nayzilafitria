
<html lang="id">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>SMK AL HIKMAH BATAM - Website Resmi</title>
<style>
  * {
    margin: 0; padding: 0; box-sizing: border-box;
  }
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #0b2447;
    color: #e1e8f0;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
  }
  header {
    background: #144272;
    display: flex;
    justify-content: flex-start;
    align-items: center;
    padding: 15px 30px;
    position: relative;
    box-shadow: 0 2px 6px rgba(0,0,0,0.4);
  }
  header img.logo {
    height: 50px;
    margin-right: 15px;
    border-radius: 8px;
    user-select: none;
  }
  header h1 {
    font-size: 1.8rem;
    font-weight: 700;
    letter-spacing: 2px;
    color: #f1f5f9;
    user-select: none;
  }
  nav {
    flex-grow: 1;
    margin-left: 40px;
  }
  nav ul {
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    gap: 18px;
  }
  nav ul li {
    font-weight: 600;
  }
  nav ul li a {
    color: #c9d1d9;
    text-decoration: none;
    padding: 8px 14px;
    border-radius: 6px;
    transition: background-color 0.3s ease, color 0.3s ease;
    display: block;
    white-space: nowrap;
  }
  nav ul li a:hover,
  nav ul li a.active {
    background-color: #1e4f8b;
    color: #fff;
  }
  .menu-toggle {
    width: 28px;
    height: 22px;
    display: none;
    flex-direction: column;
    justify-content: space-between;
    cursor: pointer;
    z-index: 1001;
  }
  .menu-toggle span {
    display: block;
    height: 3px;
    background: #c9d1d9;
    border-radius: 3px;
    transition: all 0.3s ease;
  }
  nav.mobile-active ul {
    display: flex !important;
    flex-direction: column;
    position: absolute;
    top: 58px;
    right: 30px;
    background: #144272;
    border-radius: 8px;
    box-shadow: 0 8px 20px rgba(0,0,0,0.4);
    width: 220px;
    animation: slideDown 0.25s ease forwards;
    z-index: 999;
  }
  nav.mobile-active ul li {
    padding: 12px 20px;
  }
  nav.mobile-active ul li a {
    padding: 6px 0;
  }
  @keyframes slideDown {
    from {
      opacity: 0;
      transform: translateY(-15px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
  main {
    flex-grow: 1;
    max-width: 960px;
    margin: 30px auto 60px;
    padding: 0 20px;
  }
  section {
    display: none;
  }
  section.active {
    display: block;
    animation: fadeInContent 0.3s ease forwards;
  }
  @keyframes fadeInContent {
    from {opacity: 0; transform: translateY(10px);}
    to {opacity: 1; transform: translateY(0);}
  }
  h2 {
    margin-bottom: 20px;
    border-bottom: 3px solid #1e4f8b;
    padding-bottom: 8px;
    font-weight: 700;
  }
  table {
    width: 100%;
    border-collapse: collapse;
    background-color: #1e4f8b;
    border-radius: 8px;
    overflow: hidden;
  }
  th, td {
    padding: 14px 18px;
    border: 1px solid #134270;
    text-align: left;
    color: #e1e8f0;
  }
  th {
    background-color: #134270;
  }
  form {
    max-width: 420px;
    background: #144272;
    padding: 30px;
    border-radius: 10px;
    box-shadow: 0 0 15px rgba(20,66,114,0.7);
  }
  label {
    display: block;
    margin-bottom: 8px;
    font-weight: 600;
  }
  input[type="text"],
  input[type="password"],
  textarea {
    width: 100%;
    padding: 11px 14px;
    margin-bottom: 22px;
    border: none;
    border-radius: 6px;
    font-size: 1rem;
    font-family: inherit;
  }
  input[type="submit"] {
    background-color: #1e4f8b;
    border: none;
    padding: 14px;
    width: 100%;
    color: white;
    font-weight: 700;
    cursor: pointer;
    border-radius: 6px;
    font-size: 1rem;
    transition: background-color 0.3s ease;
  }
  input[type="submit"]:hover {
    background-color: #134270;
  }
  footer {
    background: #144272;
    text-align: center;
    color: #c9d1d9;
    padding: 15px 10px;
    font-size: 0.9rem;
    margin-top: auto;
    user-select: none;
  }
  /* Gambar di section */
  section img {
    width: 100%;
    max-width: 600px;
    border-radius: 12px;
    margin-bottom: 15px;
    user-select: none;
  }
  @media (max-width: 900px) {
    nav ul {
      display: none;
    }
    .menu-toggle {
      display: flex;
    }
  }
</style>
</head>
<body>
  <header>
    <img src="https://uploads.onecompiler.io/43w7hwn73/43xrc4apr/WhatsApp%20Image%202025-09-25%20at%2015.13.39.jpeg" alt="Logo SMK Negeri 7 Batam" class="logo" />
    <h1>SMK AL HIKMAH BATAM</h1>
    <nav id="nav-menu" aria-label="Navigasi utama">
      <ul>
        <li><a href="#" class="nav-link active" data-target="home">Home</a></li>
        <li><a href="#" class="nav-link" data-target="profile">Profile</a></li>
        <li><a href="#" class="nav-link" data-target="nama-siswa">Nama Siswa</a></li>
        <li><a href="#" class="nav-link" data-target="kejuruan">Kejuruan</a></li>
        <li><a href="#" class="nav-link" data-target="program">Program</a></li>
        <li><a href="#" class="nav-link" data-target="gtk-siswa">GTK dan Siswa</a></li>
        <li><a href="#" class="nav-link" data-target="sarpras">Sarpras</a></li>
        <li><a href="#" class="nav-link" data-target="kegiatan">Kegiatan</a></li>
        <li><a href="#" class="nav-link" data-target="galeri">Galeri</a></li>
        <li><a href="#" class="nav-link" data-target="berita">Berita</a></li>
        <li><a href="#" class="nav-link" data-target="blog">Blog</a></li>
        <li><a href="#" class="nav-link" data-target="kontak">Kontak</a></li>
        <li><a href="#" class="nav-link" data-target="login">Login</a></li>
      </ul>
    </nav>
    <div class="menu-toggle" id="menu-toggle" aria-label="Toggle menu" aria-expanded="false" role="button" tabindex="0">
      <span></span>
      <span></span>
      <span></span>
    </div>
  </header>

  <main>
    <section id="home" class="active">
      <h2>Selamat Datang di SMK AL HIKMAH BATAM</h2>
      <p>Website resmi sekolah SMK Al Hikmah Batam, tempat menimba ilmu dan berprestasi.</p>
      <p>Kami berkomitmen memberikan pendidikan terbaik dengan fasilitas lengkap dan tenaga pengajar profesional. Menjadikan siswa/i berakhlak mulia, bertaqwa kepada Tuhan Yang Maha Esa dan berprestasi dalam bidang akademik maupun non akademik.</p>
    </section>

    <section id="profile">
      <h2>Profil Sekolah</h2>
      <p>SMK Al Hikmah Batam didirikan pada tahun 2005 dan berlokasi di Batam, Kepulauan Riau. Sekolah kami memiliki visi untuk mencetak lulusan yang siap kerja dan berkompeten di bidangnya dan siap berkompetisi di dunia kerja.</p>
      <ul>
        <li>Alamat: Jl. Pendidikan No.7, Batam</li>
        <li>Telepon: (0778) 123456</li>
        <li>Email: info@smkalhikmahbatam.sch.id</li>
      </ul>

      <hr style="margin: 30px 0; border-color: #1e4f8b;" />

      <h3>Profil Kepala Sekolah</h3>
      <div style="display: flex; align-items: center; gap: 20px; flex-wrap: wrap;">
        <img src="https://uploads.onecompiler.io/43w7hwn73/43wbrfzfz/WhatsApp%20Image%202025-09-11%20at%2003.40.25.jpeg" alt="Foto Kepala Sekolah" style="width: 150px; border-radius: 12px; box-shadow: 0 0 8px rgba(0,0,0,0.3);" />
        <div>
          <p><strong>Nama:</strong> Drs.Nayzila Fitria Ramadani, M.Pd</p>
          <p><strong>Jabatan:</strong> Kepala Sekolah SMK AL HIKMAH Batam</p>
          <p>Drs.Nayzila Fitria Ramadani, M.Pd adalah kepala sekolah yang berpengalaman dengan lebih dari 20 tahun di dunia pendidikan. Beliau berkomitmen meningkatkan kualitas pendidikan dan membangun karakter siswa agar siap menghadapi tantangan masa depan.</p>
        </div> 
      </div>
    </section>

    <section id="nama-siswa">
      <h2>Daftar Nama Siswa</h2>
      <table>
        <thead>
          <tr><th>No</th><th>Nama</th><th>Kelas</th><th>Kejuruan</th></tr>
        </thead>
        <tbody>
          <tr><td>1</td><td>Andi Saputra</td><td>X RPL 1</td><td>Rekayasa Perangkat Lunak</td></tr>
          <tr><td>2</td><td>Siti Rahma</td><td>X Multimedia 2</td><td>Multimedia</td></tr>
          <tr><td>3</td><td>Budi Santoso</td><td>X Akuntansi 1</td><td>Akuntansi</td></tr>
        </tbody>
      </table>
      <h2>Jumlah siswa</h2>
     <h3 style="text-align:center; color:#1e293b; margin-bottom:15px;">Jumlah siswa</h3>
  <div class="nama-siswa">
    <div class="nama-siswa"> 1.250 siswa</div>
    <div class="bar"><div class="bar-fill" data-fill="90%"></div></div>
  </div>
    </section>

    <section id="kejuruan">
    <h3>Program Keahlian:</h3>
    <div class="grid-programs">
       <h4>Teknik Komputer & Jaringan</h4>
      <div class="program" tabindex="0" role="button" aria-label="Teknik Komputer dan Jaringan">
        <img src="https://uploads.onecompiler.io/43w7hwn73/43xrnye3d/WhatsApp%20Image%202025-09-25%20at%2017.24.07.jpeg" alt="Foto Teknik Komputer & Jaringan" />
       
      </div>
      <h4>Rekayasa Perangkat Lunak</h4>
      <div class="program" tabindex="0" role="button" aria-label="Rekayasa Perangkat Lunak">
        <img src="https://uploads.onecompiler.io/43w7hwn73/43xrnye3d/WhatsApp%20Image%202025-09-25%20at%2017.24.07%20(1).jpeg" alt="Foto Rekayasa Perangkat Lunak" />
        
      </div>
      <h5>Elektronika Industri</h5>
      <div class="program" tabindex="0" role="button" aria-label="Elektronika Industri">
        <img src="https://uploads.onecompiler.io/43w7hwn73/43xrnye3d/WhatsApp%20Image%202025-09-25%20at%2017.24.08.jpeg" alt="Foto Elektronika Industri" />
      </div>
    </div>
  </div>
    </section>

    <section id="program">
      <h2>Program Sekolah</h2>
      <p>Berbagai program unggulan yang mendukung pengembangan kompetensi siswa.</p>
      
    </section>

    <section id="gtk-siswa">
      <h2>GTK dan Siswa</h2>
      <p>Tenaga Kependidikan dan Guru yang profesional serta siswa yang aktif dan kreatif.</p>
      
      <h4><a href="#">Pengajar</a></h4>
       <span class="Pengajar"><span><span>
      <article class="gtk-siswa" tabindex="0" role="article" aria-label="Pengajar">
        <img src="https://uploads.onecompiler.io/43w7hwn73/43xrnye3d/WhatsApp%20Image%202025-09-25%20at%2017.05.35%20(1).jpeg" alt="Gambar Pengajar" />
       
        
      </article>
    <h4><a href="#">Pustakawan</a></h4>
    <span class="Pustakawan"><span>
      <article class="gtk-siswa" tabindex="0" role="article" aria-label="Pustakawan">
        <img src="https://uploads.onecompiler.io/43w7hwn73/43xrnye3d/WhatsApp%20Image%202025-09-25%20at%2017.05.35.jpeg" alt="Gambar Pustakawan" />
        
       
      </article>
      
      
    </section>

    <section id="sarpras">
      <h2>Sarana dan Prasarana</h2>
      <img src="https://uploads.onecompiler.io/43w7hwn73/43xrc4apr/WhatsApp%20Image%202025-09-25%20at%2015.05.16%20(1).jpeg" alt="Sarana dan Prasarana" />
      <p>Fasilitas lengkap seperti laboratorium komputer, perpustakaan, dan ruang kelas yang nyaman.</p>
    </section>

    <section id="kegiatan">
      <h2>Kegiatan Sekolah</h2>
      <p>Beragam kegiatan ekstrakurikuler dan acara tahunan yang memperkaya pengalaman belajar siswa.</p>
      <h3>Ekstrakurikuler Sepak Bola</h3>
      <p>Program latihan sepak bola rutin untuk mengembangkan kemampuan teknik dan kerja sama tim siswa.</p>
    </div>
    
    
      <h3>Ekskul Paduan Suara</h3>
      <p>Latihan vokal dan penampilan musik untuk membentuk grup paduan suara sekolah yang solid dan berbakat.</p>
    </div>
    
    
      <h3>Klub Robotik</h3>
      <p>Pelatihan membuat dan memprogram robot untuk meningkatkan keterampilan teknologi dan kreativitas siswa.</p>
    </div>
    </section>

    <section id="galeri">
      <h2>Galeri Foto</h2>
      <img src="https://uploads.onecompiler.io/43w7hwn73/43xrc4apr/WhatsApp%20Image%202025-09-25%20at%2015.05.16.jpeg" alt="Galeri Foto" />
    </section>

    <section id="berita">
     <h3>Berita & Pengumuman Terbaru</h3>
    <div class="berita-list">
      <article class="berita-item" tabindex="0" role="article" aria-label="Pengumuman PPDB 2025">
        <img src="https://uploads.onecompiler.io/43w7hwn73/43xrnye3d/WhatsApp%20Image%202025-09-25%20at%2017.50.33.jpeg" alt="Gambar Berita Pengumuman PPDB 2025" />
        <h4><a href="#">Pengumuman PPDB 2025</a></h4>
        <span class="date">25 Agustus 2025</span>
      </article>
      <article class="berita-item" tabindex="0" role="article" aria-label="Prestasi Lomba Siswa">
        <img src="https://uploads.onecompiler.io/43w7hwn73/43xrnye3d/WhatsApp%20Image%202025-09-25%20at%2017.50.32.jpeg" alt="Gambar Berita Prestasi Lomba Siswa" />
        <h4><a href="#">Prestasi Lomba Siswa</a></h4>
        <span class="date">10 Juli 2025</span>
      </article>
    </div>
  </div>
   </section>
   
    <section id="blog">
      <h2>Blog Sekolah</h2>
      <p>Artikel dan cerita seputar kegiatan dan prestasi siswa.</p>
        <img src="https://uploads.onecompiler.io/43w7hwn73/43xrc4apr/WhatsApp%20Image%202025-09-25%20at%2015.13.39.jpeg" alt="Logo SMK Al Hikmah" style="max-width:150px; margin-bottom:20px; border-radius:10px;">
  <h1>Selamat Datang di Blog SMK Al Hikmah</h1>


    </section>

    <section id="kontak">
      <h2>Kontak Kami</h2>
      <form id="contact-form" aria-label="Form kontak">
        <label for="name">Nama:</label>
        <input type="text" id="name" name="name" required placeholder="Masukkan nama Anda" />
       
        <label for="email">Email:</label>
        <input type="text" id="email" name="email" required placeholder="Masukkan email Anda" />

        <label for="message">Pesan:</label>
        <textarea id="message" name="message" rows="5" required placeholder="Tulis pesan Anda"></textarea>

        <input type="submit" value="Kirim Pesan" />
      </form>
    </section>

    <section id="login">
      <h2>Login Pengguna</h2>
      <form id="login-form" aria-label="Form login">
        <label for="username">Username:</label>
        <input type="text" id="username" name="username" required placeholder="Masukkan username" />

        <label for="password">Password:</label>
        <input type="password" id="password" name="password" required placeholder="Masukkan password" />

        <input type="submit" value="Login" />
      </form>
    </section>
  </main>

  <footer>
    &copy; 2025 SMK Al Hikmah Batam. All rights reserved.
  </footer>

<script>
  // Navigasi SPA
  const navLinks = document.querySelectorAll('.nav-link');
  const sections = document.querySelectorAll('main section');

  function activateSection(targetId) {
    sections.forEach(section => {
      section.classList.toggle('active', section.id === targetId);
    });
    navLinks.forEach(link => {
      link.classList.toggle('active', link.dataset.target === targetId);
    });
  }

  navLinks.forEach(link => {
    link.addEventListener('click', e => {
      e.preventDefault();
      const target = link.dataset.target;
      activateSection(target);

      // Tutup menu mobile jika terbuka
      if (navMenu.classList.contains('mobile-active')) {
        navMenu.classList.remove('mobile-active');
        menuToggle.setAttribute('aria-expanded', 'false');
      }
    });
  });

  // Menu toggle untuk mobile
  const menuToggle = document.getElementById('menu-toggle');
  const navMenu = document.getElementById('nav-menu');

  menuToggle.addEventListener('click', () => {
    navMenu.classList.toggle('mobile-active');
    const expanded = menuToggle.getAttribute('aria-expanded') === 'true';
    menuToggle.setAttribute('aria-expanded', String(!expanded));
  });

  // Accessibility: keyboard toggle menu
  menuToggle.addEventListener('keydown', e => {
    if (e.key === 'Enter' || e.key === ' ') {
      e.preventDefault();
      menuToggle.click();
    }
  });

  // Form submit handlers (contoh sederhana)
  document.getElementById('contact-form').addEventListener('submit', e => {
    e.preventDefault();
    alert('Terima kasih sudah mengirim pesan!');
    e.target.reset();
  });

  document.getElementById('login-form').addEventListener('submit', e => {
    e.preventDefault();
    alert('Login berhasil (simulasi).');
    e.target.reset();
  });
</script>
</body>
</html>
