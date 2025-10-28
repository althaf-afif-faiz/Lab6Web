# Lab6Web
---   
# Praktikum 6 

## 👤 Identitas
- **Nama:** Althaf Afif Faiz  
- **NIM:** 312410404  
- **Mata Kuliah:** Pemrograman Web 1     
- **Dosen Pengampu:** _Agung Nugroho, S.Kom., M.Kom._  

---

## Mengerjakan Latihan Praktikum 6 :    

### Code Program :    
<img width="1748" height="4244" alt="code latihan" src="https://github.com/user-attachments/assets/670e7b1f-583e-427d-b5c6-ed3222301ee8" />

### Ouput :     
<img width="1357" height="694" alt="image" src="https://github.com/user-attachments/assets/58d6cc70-d096-43ca-a6cb-4be58c2a669e" />


---   

- **Pertanyaan dan Tugas** 
1. Refactor Layout Praktikum 4    
Ambil layout web sederhana dari Praktikum 4. Buat ulang layout tersebut menggunakan    
Bootstrap Grid System.      
○ Gunakan <nav> Bootstrap untuk bagian navigasi     
○ Gunakan class .row dan .col-md-8 untuk main content dan .col-md-4 untuk sidebar    
○ Gunakan komponen .card Bootstrap untuk menggantikan .widget-box     
○ Gunakan komponen .card untuk menggantikan .box (bagian "Heading" yang berisi 3     
kolom)     
○ Anda tidak diperbolehkan menggunakan CSS float atau clear manual.    

2. Refactor Form Praktikum 5     
Ambil salah satu form dari Praktikum 5 (misalnya Form Input 23atau Form Button 24).      
Buat ulang form tersebut agar terlihat rapi menggunakan class-class form Bootstrap (.form-    
control, .form-label, .btn).    

3. Tugas: Buat Halaman Portfolio Sederhana
Buat satu halaman HTML baru (portfolio.html) menggunakan Bootstrap yang berisi:
a. Sebuah Navbar di bagian atas.
b. Sebuah section "Tentang Saya" di dalam .container dengan 1 baris (.row) dan 2 kolom
(.col):
* Kolom kiri (.col-md-4) berisi foto Anda (gunakan <img> dengan class .img-fluid).
* Kolom kanan (.col-md-8) berisi nama dan deskripsi diri Anda.
c. Sebuah section "Portfolio Saya" di dalam .container dengan 1 baris (.row) dan 3 kolom
(.col-md-4):
* Setiap kolom berisi satu komponen .card yang merepresentasikan satu proyek (beri
gambar dummy dan deskripsi singkat).

---     

## 1. Refactor Layout Praktikum 4      

### Code Program :    
<img width="1988" height="6980" alt="code praktikum 4" src="https://github.com/user-attachments/assets/19bd8ba2-ffe8-4b94-9944-470baa9ffb3d" />

### Output :    
<img width="661" height="578" alt="image" src="https://github.com/user-attachments/assets/9103a0f8-e404-4cf5-847b-034a2ef46360" />


## 2. Refactor Form Praktikum 5  

### Code Program :     
<img width="2730" height="5914" alt="code praktikum 5" src="https://github.com/user-attachments/assets/7082cbc9-7eb0-44d3-971b-7e119c6fb119" />

### Output :    
<img width="1351" height="679" alt="image" src="https://github.com/user-attachments/assets/b8d8fa4e-8edc-412c-b217-b25b06bdfc9f" />

<img width="1349" height="677" alt="image" src="https://github.com/user-attachments/assets/620ae864-aeb8-4c8a-8b71-e8d873f7c15e" />

## 3. Tugas:   
### Buat Halaman Portfolio Sederhana :       

### Code Program :    
<img width="2192" height="8992" alt="code portofolio" src="https://github.com/user-attachments/assets/718198ec-f8b8-4990-a6d2-ba07ed8852cd" />

### Output :      
#### Output dari navbar Tentang saya :     
<img width="1354" height="687" alt="image" src="https://github.com/user-attachments/assets/e116230b-9e03-4882-b229-90d662e6e3d2" />

#### Output dari navbar portofolio :       
<img width="1347" height="684" alt="image" src="https://github.com/user-attachments/assets/56d150e2-5ebf-4cf1-ba90-5b315a6504f2" />

## Penjelasan Tugas :    
### Bootstrap
Bootstrap adalah framework front-end berbasis HTML, CSS, dan JavaScript yang digunakan untuk mempercepat pengembangan tampilan web responsif.  
Bootstrap menyediakan komponen siap pakai seperti:
- `.navbar` – untuk navigasi
- `.container`, `.row`, `.col` – untuk layout grid system
- `.card` – untuk menampilkan konten bergaya panel

### Grid System
Sistem grid Bootstrap membagi halaman menjadi 12 kolom fleksibel, memungkinkan penataan elemen agar tetap responsif di berbagai ukuran layar.

---

## Implementasi

File utama: **`portfolio.html`**

###  Struktur Halaman
Halaman ini dibagi menjadi beberapa bagian utama:
1. **Navbar** di bagian atas halaman.  
2. **Section "Tentang Saya"** — menampilkan foto dan deskripsi diri.  
3. **Section "Portfolio Saya"** — menampilkan tiga proyek dalam bentuk card.  
4. **Footer** di bagian bawah halaman.

---

## Cuplikan Kode Penting

### 1️. Navbar
```html
<nav class="navbar navbar-expand-lg navbar-dark fixed-top shadow-sm">
  <div class="container">
    <a class="navbar-brand" href="#">AfifPortfolio</a>
    ...
  </div>
</nav>
```

### 2️. Tentang Saya
```
<section id="tentang" class="text-center">
  <div class="container mt-5 pt-5">
    <div class="row align-items-center justify-content-center">
      <div class="col-md-4">
        <img src="foto.jpg" />
      </div>
      <div class="col-md-7 text-md-start">
        <h2 class="fw-bold">Althaf Afif Faiz</h2>
        <p class="lead text-muted">
          Saya seorang mahasiswa yang memiliki minat besar dalam pengembangan web dan desain
          antarmuka pengguna...
        </p>
      </div>
    </div>
  </div>
</section>
``` 

### 3️. Portfolio Saya    
```
<section id="portfolio">
  <div class="container">
    <h2 class="section-title">Portfolio Saya</h2>
    <div class="row g-4">
      <div class="col-md-4">
        <div class="card shadow-sm h-100">
          <img src="https://images.unsplash.com/photo-1581091215367-59ab6b3c94a9" class="card-img-top" />
          <div class="card-body">
            <h5 class="card-title fw-semibold">Website Sekolah</h5>
            <p class="card-text text-muted">Website informatif sekolah dengan fitur berita...</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
```

