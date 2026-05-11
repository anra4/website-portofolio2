<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio Anra</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <link rel="shortcut icon" href="foto3.png" type="image/x-icon">
    <style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: 'Montserrat', sans-serif;
    }

    body {
        background-color: #ffffff;
        overflow-x: hidden;
    }

    /* Container Utama */
    .hero-container {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 50px 10%;
        min-height: 85vh;
        gap: 40px; /* Jarak antara teks dan gambar */
    }

    /* Bagian Kiri: Teks */
    .hero-text {
        flex: 1;
    }

    .hero-text h1 {
        font-size: 3.5rem;
        color: #0056b3;
        line-height: 1.1;
        margin-bottom: 20px;
    }

    .hero-text h1 span {
        color: #333;
    }

    .hero-text p {
        font-size: 1.1rem;
        color: #555;
        max-width: 500px;
        margin-bottom: 15px;
        line-height: 1.6;
    }

    /* Tombol */
    .btn-group {
        margin-top: 30px;
        display: flex;
        gap: 15px; /* Memberi jarak antar tombol tanpa margin manual */
    }

    .btn-cv {
        display: inline-block;
        background-color: #0056b3;
        color: white;
        padding: 12px 25px;
        text-decoration: none;
        border-radius: 5px;
        font-weight: bold;
        font-size: 1rem;
        transition: background-color 0.3s, transform 0.2s;
        text-align: center;
    }

    .btn-cv:hover {
        background-color: #003d80;
        transform: translateY(-3px);
    }

    /* Bagian Kanan: Gambar */
    .hero-image {
        flex: 1;
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
    }

    .blue-box {
        background-color: #0056b3;
        width: 100%;
        max-width: 350px;
        height: 400px;
        border-radius: 30px;
        position: relative;
        display: flex;
        align-items: flex-end;
        justify-content: center;
        overflow: hidden;
        z-index: 1;
    }

    .blue-box img {
    width: 100%;      /* Foto memenuhi lebar kotak */
    height: 100%;     /* Foto memenuhi tinggi kotak */
    object-fit: cover; /* Foto akan terpotong rapi tanpa gepeng/ketarik */
    object-position: top; /* Fokus ke area wajah (atas) */
}

    .circle-yellow {
        width: 60px; height: 60px;
        background-color: #f1c40f;
        border-radius: 50%;
        position: absolute;
        left: -20px; bottom: 10%;
        z-index: 2;
    }

    .circle-red {
        width: 80px; height: 80px;
        background-color: #e73cc2;
        border-radius: 50%;
        position: absolute;
        right: -10px; top: 5%;
        z-index: 0;
    }

    /* Menu Ikon Bawah */
    /* Bagian Bawah: Menu Ikon Bulat */
.icon-menu {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 40px;          /* Jarak antar ikon diperlebar */
    padding: 60px 0;    /* Area menu dibuat lebih lega */
    background-color: #fff;
    flex-wrap: wrap;
}

.icon-item {
    width: 150px;        /* Ukuran lingkaran diperbesar (dari sebelumnya kecil) */
    height: 150px;
    background-color: #0056b3;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    font-size: 2.5rem;   /* Ukuran simbol di dalam lingkaran diperbesar */
    text-decoration: none;
    cursor: pointer;
    transition: all 0.3s ease;
    box-shadow: 0 10px 20px rgba(0,0,0,0.1); /* Tambah bayangan halus agar mewah */
}

.icon-item:hover {
    transform: scale(1.2); /* Efek membesar saat kursor menempel */
    background-color: #003d80;
    box-shadow: 0 15px 30px rgba(0,0,0,0.2);
}

/* Penyesuaian untuk HP agar tidak terlalu raksasa */
@media (max-width: 768px) {
    .icon-menu {
        gap: 20px;
        padding: 40px 10%;
    }
    .icon-item {
        width: 80px;
        height: 80px;
        font-size: 1.8rem;
    }
}
    
.footer-copyright {
    text-align: center;
    padding: 25px 0; /* Sedikit lebih lebar agar lega */
    background-color: #f1f1f1; 
    color: #333;             /* Warna diganti ke lebih gelap agar jelas */
    font-size: 1.1rem;       /* Ukuran standar dinaikkan (sebelumnya 0.9) */
    border-top: 1px solid #ddd;
    margin-top: 30px;
    font-weight: 500;        /* Sedikit lebih tebal */
}

/* Responsif untuk HP */
@media (max-width: 768px) {
    .footer-copyright {
        font-size: 1rem;     /* Di HP tidak terlalu kecil (sebelumnya 0.8) */
        padding: 20px 15px;
    }
}
   
</style>
</head>
<body>

    <section class="hero-container">
        <div class="hero-text">
            <h1>Halo, Saya<br><span>Antika Rahayu Shaqila</span></h1>
            
            <p>
                Seorang lulusan <strong>SMK NEGERI 4 KUNINGAN</strong> yang disiplin dan berorientasi pada detail. 
                Memiliki pengalaman dalam bekerja dalam tim.
            </p>
            
            <p>
                Saya berkomitmen untuk memberikan kontribusi positif bagi perusahaan melalui keterampilan 
                manajemen waktu yang baik serta kemauan untuk terus belajar hal baru.
            </p>
            
            <div class="btn-group">
            <a href="https://mail.google.com/mail/?view=cm&fs=1&to=antikarash58@gmail.com" class="btn-cv">Kirim Email</a>
             <a href="https://drive.google.com/file/d/1-KElW5CXP4TgGOclFxK6niMsfvj1UHCe/view?usp=cv Antika Rahayu Shaqila.pdf" target="_blank" class="btn-                       cv">Lihat / Download CV</a>
           </div>
        </div>

        <div class="hero-image">
            <div class="circle-yellow"></div>
            <div class="blue-box">
                <img src="foto2.png" alt="Foto Profesional">
            </div>
            <div class="circle-red"></div>
        </div>
    </section>

    <div class="icon-menu">
        <a href="profil.html" class="icon-item" title="Tentang Saya">👤</a>
        
        <a href="pendidikan.html" class="icon-item" title="Pendidikan">🎓</a>
        
        <a href="pengalaman.html" class="icon-item" title="Pengalaman Kerja">💼</a>
        <a href="keahlian.html" class="icon-item" title="Keahlian">🛠️</a>
        <a href="kontak.html" class="icon-item" title="Kontak">📞</a>
    </div>
    <footer class="footer-copyright">
    <p>&copy; 2026 Anra. All Rights Reserved.</p>
</footer>
</body>
</html>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profil Lengkap - [Nama Anda]</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Montserrat', sans-serif;
        }

        body {
            background-color: #f0f4f8;
            color: #333;
            padding: 40px 20px;
            line-height: 1.6;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
        }

        header {
            text-align: center;
            margin-bottom: 40px;
        }

        header h1 {
            color: #0056b3;
            font-size: 2.5rem;
        }

        /* Gaya Kotak Informasi (Section) */
        .section-box {
            background: #fff;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.05);
            margin-bottom: 20px;
            border-left: 5px solid #0056b3; /* Aksen garis biru di kiri */
        }

        .section-box h2 {
            color: #0056b3;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .back-btn {
            display: inline-block;
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #0056b3;
            color: white;
            text-decoration: none;
            border-radius: 30px;
            font-weight: bold;
            transition: 0.3s;
        }

        .back-btn:hover {
            background-color: #003d80;
            transform: translateX(-5px);
        }

        /* List untuk Hobi agar rapi */
        .hobi-list {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            list-style: none;
            margin-top: 10px;
        }

        .hobi-item {
            background: #e1ecf7;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            color: #0056b3;
            font-weight: bold;
        }
     .footer-copyright {
      text-align: center;
      padding: 25px 0; /* Sedikit lebih lebar agar lega */
      background-color: #f1f1f1; 
      color: #333;             /* Warna diganti ke lebih gelap agar jelas */
      font-size: 1.1rem;       /* Ukuran standar dinaikkan (sebelumnya 0.9) */
      border-top: 1px solid #ddd;
     margin-top: 30px;
     font-weight: 500;        /* Sedikit lebih tebal */
     }

       /* Responsif untuk HP */
       @media (max-width: 768px) {
      .footer-copyright {
        font-size: 1rem;     /* Di HP tidak terlalu kecil (sebelumnya 0.8) */
        padding: 20px 15px;
       }
      } 
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>Tentang Saya</h1>
            <p>Mengenal lebih dekat perjalanan profesional dan pribadi saya.</p>
        </header>

        <div class="section-box">
            <h2>👤 Biografi Singkat</h2>
            <p>
                Saya adalah seorang lulusan SMK NEGERI 4 KUNINGAN yang memiliki ketertarikan besar dalam dunia berbagai bidang operasional dan industri kreatif. 
                Lahir dan besar di Cirebon, Jawa Barat, saya terbiasa bekerja keras dan menghargai nilai-nilai kejujuran dalam lingkungan kerja.
            </p>
        </div>

        <div class="section-box">
            <h2>🎨 Hobi & Ketertarikan</h2>
            <p>Di waktu senggang, saya senang mengeksplorasi kreativitas dan menjaga keseimbangan hidup melalui:</p>
            <ul class="hobi-list">
                <li class="hobi-item">Membaca Novel </li>
                <li class="hobi-item">Berimajinasi </li>
                <li class="hobi-item">Olahraga Sepeda</li>
                <li class="hobi-item">Membuat prakarya</li>
            </ul>
        </div>

        <div class="section-box">
            <h2>🚀 Motivasi Kerja</h2>
            <p>
            Bekerja bukan hanya tentang menyelesaikan tugas, tetapi tentang memberikan nilai tambah dan solusi di setiap kesempatan
            </p>
        </div>

        <div style="text-align: center;">
            <a href="portofolio.html" class="back-btn">← Kembali ke Halaman Utama</a>
        </div>
    </div>
     <footer class="footer-copyright">
    <p>&copy; 2026 Anra. All Rights Reserved.</p>
</footer>

</body>
</html>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profil Lengkap - [Nama Anda]</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Montserrat', sans-serif;
        }

        body {
            background-color: #f0f4f8;
            color: #333;
            padding: 40px 20px;
            line-height: 1.6;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
        }

        header {
            text-align: center;
            margin-bottom: 40px;
        }

        header h1 {
            color: #0056b3;
            font-size: 2.5rem;
        }

        /* Gaya Kotak Informasi (Section) */
        .section-box {
            background: #fff;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.05);
            margin-bottom: 20px;
            border-left: 5px solid #0056b3; /* Aksen garis biru di kiri */
            display: flex; 
            align-items: flex-start; /* Sejajar dari atas */
            justify-content: space-between; /* Memberi jarak antara teks dan peta */
            gap: 20px; /* Jarak antara teks dan peta */
            flex-wrap: wrap; /* Agar jika di layar HP, peta pindah ke bawah otomatis */
        }
    

        .section-box h2 {
            color: #0056b3;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .badge-lulus {
        background-color: #27ae60; /* Warna Hijau */
        color: white;
        padding: 4px 12px;
        border-radius: 20px;
        font-size: 0.8rem;
        font-weight: bold;
        vertical-align: middle;
        margin-left: 10px;
        display: inline-block;
    }

    /* Memastikan teks informasi sejajar rapi */
    

        .back-btn {
            display: inline-block;
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #0056b3;
            color: white;
            text-decoration: none;
            border-radius: 30px;
            font-weight: bold;
            transition: 0.3s;
        }

        .back-btn:hover {
            background-color: #003d80;
            transform: translateX(-5px);
        }

        /* List untuk Hobi agar rapi */
        .hobi-list {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            list-style: none;
            margin-top: 10px;
        }

        .hobi-item {
            background: #e1ecf7;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            color: #0056b3;
            font-weight: bold;
        }

         .footer-copyright {
    text-align: center;
    padding: 25px 0; /* Sedikit lebih lebar agar lega */
    background-color: #f1f1f1; 
    color: #333;             /* Warna diganti ke lebih gelap agar jelas */
    font-size: 1.1rem;       /* Ukuran standar dinaikkan (sebelumnya 0.9) */
    border-top: 1px solid #ddd;
    margin-top: 30px;
    font-weight: 500;        /* Sedikit lebih tebal */
}

/* Responsif untuk HP */
@media (max-width: 768px) {
    .footer-copyright {
        font-size: 1rem;     /* Di HP tidak terlalu kecil (sebelumnya 0.8) */
        padding: 20px 15px;
    }
}
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>Tentang Pendidikan</h1>
            <p>Mengenal lebih dekat perjalanan profesional dan pribadi saya.</p>
        </header>

        <div class="section-box">
            <h2>👩‍🎓SD Negeri 1 Tanjunganom<span class="badge-lulus">Lulus-2020</span></h2>
            <p>
              Nama	                    :	SD NEGERI 1 TANJUNG ANOM KECAMATAN PASALEMAN<br>
 	          NPSN	                    :	20215473<br>
 	          Alamat	                :	Jl. Raya Tanjunganom Kec. Pasaleman Kab. Cirebon<br>
 	          Desa/Kelurahan	        :	TANJUNG ANOM<br>
              Kecamatan/Kota (LN)	    :	KEC. PASALEMAN<br>
              Kab.-Kota/Negara (LN)	    :	KAB. CIREBON<br>
 	          Propinsi/Luar Negeri (LN)	:	PROV. JAWA BARAT<br>
 	          Status Sekolah	        :	NEGERI<br>
              Bentuk Pendidikan	        :	SD<br>
 	          Jenjang Pendidikan	    :	DIKDAS<br> 
            </p>

           <div class="maps-container">
             <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3960.560376761568!2d108.7559303748228!3d-6.943024893057075!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e6f090aeb9566a3%3A0x34c206c48ef7d2d2!2sSDN%201%20Tanjung%20Anom!5e0!3m2!1sen!2sus!4v1778470558539!5m2!1sen!2sus" width="200" height="200" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
             </div>
            
        </div>
        <div class="section-box">
            <h2>👩‍🎓SMP AN-NUUR PASALEMAN<span class="badge-lulus">Lulus-2023</span></h2>
            <p>
 	         Alamat	                    :	Jl. Raya Pasaleman No. 2<br>
             NPSN	                    :		20214810<br>
 	         Desa/Kelurahan          	:	CIKEUSIK<br>
 	         Kecamatan/Kota (LN)	    :	PASALEMAN<br>
 	         Kab.-Kota/Negara (LN)	    :	KAB. CIREBON<br>
 	         Propinsi/Luar Negeri (LN)	:	PROV. JAWA BARAT<br>
 	         Status Sekolah	            :	SWASTA<br>
 	         Bentuk Pendidikan      	:	SMP<br>
 	         Jenjang Pendidikan     	:	DIKDAS
            </p>

           <div class="maps-container">
           <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3960.7340147347854!2d108.72667707781096!3d-6.9223665752276275!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e6f093b34325409%3A0x2147f8eb4e8fb230!2sSMP%20AN-NUUR%20PASALEMAN!5e0!3m2!1sen!2sus!4v1778472318866!5m2!1sen!2sus" width="200" height="200" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
           </div>
            
        </div>  
         <div class="section-box">
            <h2>👩‍🎓SMK NEGERI 4 KUNINGAN<span class="badge-lulus">Lulus-2026</span></h2>
            <p>
 	         Alamat	                    :	JL. RAYA CIKEUSIK - CIDAHU<br>
             NPSN	                    :	20246369<br>
 	         Desa/Kelurahan          	:	CIKEUSIK<br>
 	         Kecamatan/Kota (LN)	    :	KEC. CIDAHU<br>
 	         Kab.-Kota/Negara (LN)	    :	KAB. KUNINGAN<br>
 	         Propinsi/Luar Negeri (LN)	:	PROV. JAWA BARAT<br>
 	         Status Sekolah	            :	NEGERI<br>
 	         Bentuk Pendidikan      	:	SMK<br>
 	         Jenjang Pendidikan     	:	DIKMEN
            </p>

           <div class="maps-container">
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3960.4519815934177!2d108.68152037482288!3d-6.955890093044438!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e6f0e97e9beddcb%3A0x2fd17d5f9eaf9d66!2sSMK%20Negeri%204%20Kuningan!5e0!3m2!1sen!2sus!4v1778470791876!5m2!1sen!2sus" width="200" height="200" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
     </div>
            
        </div>

        <div style="text-align: center;">
            <a href="portofolio.html" class="back-btn">← Kembali ke Halaman Utama</a>
        </div>
    </div>
     <footer class="footer-copyright">
    <p>&copy; 2026 Anra. All Rights Reserved.</p>
</footer>
</body>
</html>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profil Lengkap - [Nama Anda]</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Montserrat', sans-serif;
        }

        body {
            background-color: #f0f4f8;
            color: #333;
            padding: 40px 20px;
            line-height: 1.6;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
        }

        header {
            text-align: center;
            margin-bottom: 40px;
        }

        header h1 {
            color: #0056b3;
            font-size: 2.5rem;
        }

        /* Gaya Kotak Informasi (Section) */
        .section-box {
            background: #fff;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.05);
            margin-bottom: 20px;
            border-left: 5px solid #0056b3; /* Aksen garis biru di kiri */
            display: flex; 
            align-items: flex-start; /* Sejajar dari atas */
            justify-content: space-between; /* Memberi jarak antara teks dan peta */
            gap: 20px; /* Jarak antara teks dan peta */
            flex-wrap: wrap; /* Agar jika di layar HP, peta pindah ke bawah otomatis */
        }
    

        .section-box h2 {
            color: #0056b3;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .badge-lulus {
        background-color: #27ae60; /* Warna Hijau */
        color: white;
        padding: 4px 12px;
        border-radius: 20px;
        font-size: 0.8rem;
        font-weight: bold;
        vertical-align: middle;
        margin-left: 10px;
        display: inline-block;
    }

    /* Memastikan teks informasi sejajar rapi */
    

        .back-btn {
            display: inline-block;
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #0056b3;
            color: white;
            text-decoration: none;
            border-radius: 30px;
            font-weight: bold;
            transition: 0.3s;
        }

        .back-btn:hover {
            background-color: #003d80;
            transform: translateX(-5px);
        }

        /* List untuk Hobi agar rapi */
        .hobi-list {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            list-style: none;
            margin-top: 10px;
        }

        .hobi-item {
            background: #e1ecf7;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            color: #0056b3;
            font-weight: bold;
        }

        .footer-copyright {
    text-align: center;
    padding: 25px 0; /* Sedikit lebih lebar agar lega */
    background-color: #f1f1f1; 
    color: #333;             /* Warna diganti ke lebih gelap agar jelas */
    font-size: 1.1rem;       /* Ukuran standar dinaikkan (sebelumnya 0.9) */
    border-top: 1px solid #ddd;
    margin-top: 30px;
    font-weight: 500;        /* Sedikit lebih tebal */
}

/* Responsif untuk HP */
@media (max-width: 768px) {
    .footer-copyright {
        font-size: 1rem;     /* Di HP tidak terlalu kecil (sebelumnya 0.8) */
        padding: 20px 15px;
    }
}
    </style>
</head>
<body>

   <div class="container">
    <header>
        <h1>Pengalaman</h1>
        <p>Mengenal lebih dekat perjalanan profesional dan pribadi saya.</p>
    </header>

    <div class="section-box">
        <div class="info-text">
            <h2>Prisma Digital <br>Printing & Advertising <span class="badge-lulus">PKL Selesai</span></h2>
            <p style="color: #666; font-size: 0.9rem; margin-bottom: 10px;">
                📍 Jl. Pangeran Sutajaya, Pabuaran Lor, Cirebon<br>
                📅 <strong>Periode:</strong>27juli-29November 2023
            </p>
            
            <h4 style="color: #0056b3; margin-top: 15px; margin-bottom: 5px;">Tugas & Tanggung Jawab:</h4>
            <ul style="margin-left: 20px; font-size: 0.95rem; color: #333;">
                <li>Mendesain media promosi (Banner) menggunakan Canva.</li>
                <li>Melakukan finishing: pemotongan, pengeleman,<br>ngepres mata ayam (bolongan),<br> melipat, dan menggulung spanduk.</li>
                <li>Menjaga kebersihan dan kerapihan area operasional toko.</li>
            </ul>
        </div>
        
        <div class="maps-container">
           <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3960.894453819258!2d108.71840017482243!3d-6.903223893096104!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e6f08b64e25e3ab%3A0xd545ed2e3d703501!2sPrisma%20Digital%20Printing%20%26%20Advertising%20Pabuaran%20(CV.%20Prisma%20Masagi)!5e0!3m2!1sen!2sus!4v1778477066753!5m2!1sen!2sus" width="200" height="200" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
    </div>

    <div class="section-box">
        <div class="info-text">
            <h2>Toko Serba 35 Ribu <span class="badge-lulus">Kerja Selesai</span></h2>
            <p style="color: #666; font-size: 0.9rem; margin-bottom: 10px;">
                📍 Jl. Jatiseeng Kidul, Jatiseeng, Cirebon<br>
                📅 <strong>Periode:</strong> 6-20 Februari 2026
            </p>
            
            <h4 style="color: #0056b3; margin-top: 15px; margin-bottom: 5px;">Tugas & Tanggung Jawab:</h4>
            <ul style="margin-left: 20px; font-size: 0.95rem; color: #333;">
                <li>Visual Merchandising Assistance: Membantu penataan pakaian <br>di area pajang agar terlihat menarik bagi konsumen.</li>
                <li>Melakukan penataan barang (*display*) agar rapi dan menarik.</li>
                <li>Menjaga kebersihan area toko demi kenyamanan pengunjung.</li>
            </ul>
        </div>

        <div class="maps-container">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d330.0635719421733!2d108.74059412710756!3d-6.906710465235289!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e6f09a0c5f20b23%3A0x4e700e8d1eb2dc1d!2sToko%20Serba%2035%20Ribu!5e0!3m2!1sen!2sus!4v1778475921862!5m2!1sen!2sus" width="200" height="200" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
    </div>
      <div style="text-align: center;">
            <a href="portofolio.html" class="back-btn">← Kembali ke Halaman Utama</a>
        </div>
    
     <footer class="footer-copyright">
    <p>&copy; 2026 Anra. All Rights Reserved.</p>
</footer>

</body>
</html>

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Keahlian - Portofolio Anra</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Montserrat', sans-serif;
        }

        body {
            background-color: #f0f4f8;
            padding: 40px 20px;
        }

        .container {
            max-width: 800px;
            margin: 0 auto; /* Menengahkan container */
        }

        header {
            text-align: center;
            margin-bottom: 40px;
        }

        header h1 {
            color: #0056b3;
            font-size: 2.5rem;
        }

        /* Kotak Keahlian (Mirip Section Box Pengalaman) */
        .skill-box {
            background: #fff;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.05);
            margin-bottom: 20px;
            border-left: 8px solid #0056b3; /* Garis tebal di kiri agar sama */
            display: flex;
            align-items: center;
            gap: 25px;
        }

        .skill-icon {
            font-size: 3.5rem;
            flex-basis: 80px;
            text-align: center;
        }

        .skill-info {
            flex: 1;
        }

        .skill-info h3 {
            color: #333;
            margin-bottom: 5px;
        }

        /* Progress Bar */
        .progress-bg {
            width: 100%;
            background-color: #e1ecf7;
            border-radius: 10px;
            height: 12px;
            margin-top: 10px;
            overflow: hidden;
        }

        .progress-fill {
            height: 100%;
            background-color: #0056b3;
            border-radius: 10px;
            transition: width 1s ease-in-out;
        }

        .back-btn {
            display: inline-block;
            margin-top: 20px;
            padding: 10px 25px;
            background-color: #0056b3;
            color: white;
            text-decoration: none;
            border-radius: 30px;
            font-weight: bold;
            transition: 0.3s;
        }

        .back-btn:hover {
            background-color: #003d80;
        }

        /* Responsif HP */
        @media (max-width: 600px) {
            .skill-box {
                flex-direction: column;
                text-align: center;
            }
        }
         .footer-copyright {
    text-align: center;
    padding: 25px 0; /* Sedikit lebih lebar agar lega */
    background-color: #f1f1f1; 
    color: #333;             /* Warna diganti ke lebih gelap agar jelas */
    font-size: 1.1rem;       /* Ukuran standar dinaikkan (sebelumnya 0.9) */
    border-top: 1px solid #ddd;
    margin-top: 30px;
    font-weight: 500;        /* Sedikit lebih tebal */
}

/* Responsif untuk HP */
@media (max-width: 768px) {
    .footer-copyright {
        font-size: 1rem;     /* Di HP tidak terlalu kecil (sebelumnya 0.8) */
        padding: 20px 15px;
    }
}
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>Keahlian Saya</h1>
            <p>Kemampuan teknis yang saya kuasai.</p>
        </header>

        <div class="skill-box">
            <div class="skill-icon">🤝</div>
            <div class="skill-info">
                <h3>Kerja Sama Tim</h3>
                <p>Memiliki kemampuan komunikasi yang baik dalam lingkungan kerja.</p>
                <div class="progress-bg">
                    <div class="progress-fill" style="width:60%;"></div>
                </div>
            </div>
        </div>
        <div class="skill-box">
         <div class="skill-icon">⏳</div>
         <div class="skill-info">
          <h3>Manajemen Tekanan</h3>
          <p>Mampu tetap tenang dan produktif dalam menyelesaikan tugas meskipun di bawah tekanan atau situasi kerja yang sibuk.</p>
          <div class="progress-bg">
            <div class="progress-fill" style="width: 75%;"></div>
         </div>
         </div>
        </div>
        
        <div class="skill-box">
         <div class="skill-icon">🎯</div>
        <div class="skill-info">
        <h3>Etos Kerja & Kedisiplinan</h3>
        <p>Berkomitmen tinggi pada kejujuran, ketepatan waktu, serta selalu berusaha memberikan hasil terbaik dalam setiap tanggung jawab.</p>
        <div class="progress-bg">
            <div class="progress-fill" style="width: 90%;"></div>
        </div>
       </div>
      </div>
      <div style="text-align: center;">
            <a href="portofolio.html" class="back-btn">← Kembali ke Halaman Utama</a>
        </div>

    </div>
      <footer class="footer-copyright">
    <p>&copy; 2026 Anra. All Rights Reserved.</p>
</footer>

</body>
</html>
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kontak - Hubungi Saya</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Montserrat', sans-serif;
        }

        body {
            background-color: #f0f4f8;
            padding: 40px 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .container {
            max-width: 800px;
            width: 100%;
        }

        header {
            text-align: center;
            margin-bottom: 40px;
        }

        header h1 {
            color: #0056b3;
            font-size: 2.5rem;
        }

        .section-box {
            background: #fff;
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            border-left: 8px solid #0056b3;
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 30px;
        }

        .info-text {
            flex: 1;
        }

        .info-text h2 {
            color: #333;
            margin-bottom: 10px;
        }

        .contact-list {
            list-style: none;
            margin-top: 20px;
            font-size: 1.1rem;
        }

        .contact-list li {
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .contact-list a {
            color: #0056b3;
            text-decoration: none;
            font-weight: 500;
            transition: 0.3s;
        }

        .contact-list a:hover {
            color: #27ae60;
            text-decoration: underline;
        }

        .icon-large {
            flex-basis: 150px;
            text-align: center;
            font-size: 6rem;
            animation: float 3s ease-in-out infinite;
        }

        /* Animasi melayang agar ikon lebih hidup */
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-15px); }
        }

        .back-btn {
            margin-top: 40px;
            display: inline-block;
            padding: 12px 30px;
            background-color: #0056b3;
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            transition: 0.3s;
        }

        .back-btn:hover {
            background-color: #333;
            transform: scale(1.05);
        }

        /* Responsif untuk HP */
        @media (max-width: 600px) {
            .section-box {
                flex-direction: column-reverse;
                text-align: center;
            }
            .contact-list li {
                justify-content: center;
            }
        }
        .footer-copyright {
    text-align: center;
    padding: 25px 0; /* Sedikit lebih lebar agar lega */
    background-color: #f1f1f1; 
    color: #333;             /* Warna diganti ke lebih gelap agar jelas */
    font-size: 1.1rem;       /* Ukuran standar dinaikkan (sebelumnya 0.9) */
    border-top: 1px solid #ddd;
    margin-top: 30px;
    font-weight: 500;        /* Sedikit lebih tebal */
}

/* Responsif untuk HP */
@media (max-width: 768px) {
    .footer-copyright {
        font-size: 1rem;     /* Di HP tidak terlalu kecil (sebelumnya 0.8) */
        padding: 20px 15px;
    }
}
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>Kontak</h1>
            <p>Silakan hubungi saya melalui saluran di bawah ini.</p>
        </header>

        <div class="section-box">
            <div class="info-text">
                <h2>Mari Berdiskusi!</h2>
                <p>Saya terbuka untuk peluang kerja, magang, atau sekadar bertukar ide.</p>
                
                <ul class="contact-list">
                    <li>
                        <span>🟢</span> 
                        <strong>WhatsApp:</strong> 
                        <a href="https://wa.me/83824484713" target="_blank">+62 83824484713</a>
                    </li>
                    <li>
                        <span>📧</span> 
                        <strong>Email:</strong> 
                        <a href="mailto:antikarash58@gmail.com">antikarash58@gmail.com</a>
                    </li>
                    <li>
                        <span>📍</span> 
                        <strong>Domisili:</strong> Cirebon, Jawa Barat
                    </li>
                </ul>
            </div>

            <div class="icon-large">
                📱
            </div>
        </div>
    </div>

   <div style="text-align: center;">
            <a href="portofolio.html" class="back-btn">← Kembali ke Halaman Utama</a>
        </div>
     <footer class="footer-copyright">
    <p>&copy; 2026 Anra. All Rights Reserved.</p>
</footer>
</body>
</html>
