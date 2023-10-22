# Lab4web
# Langkah-langkah Praktikum
## Membuat Box Element
Code dan hasil
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    div {
        float:left;
        padding: 10px; 
    }
    .div1 {
        background: red;
    }
    .div2 {
        background: yellow;
    }
    .div3 {
        background: green;
    }
</style>
   
<body>
    <section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div> 
    </section>
</body>
</html>
```
<img width="359" alt="hasil1" src="https://github.com/DimasF3009/Lab4web/assets/115356128/978ab65b-5250-4342-ae6b-abc304d0fca9">

kode dan hasil
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    div {
        float:left;
        padding: 10px; 
    }
    .div1 {
        background: red;
    }
    .div2 {
        background: yellow;
    }
    .div3 {
        background: green;
    }
    .div4 {
    background-color: blue;
    clear: left;
    float: none;
    }
</style>
   
<body>
    <section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div> 
        <div class="div4">Div 4</div> 
    </section>
</body>
</html>
```
<img width="411" alt="hasil2" src="https://github.com/DimasF3009/Lab4web/assets/115356128/71f51b30-af23-4f7e-93c6-bdbdd7bf73ca">

# Membuat Layout sederhana
## Membuat folder html
```
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

</body>
</html>
```
## Membuat Navigasi
Membuat navigasi menggunakan html
```
<header><h1>Berita Masa Kini</h1></header>
    <nav>
      <ul>
        <a href="web.html" class="active">Home</a>
        <a href="#main">Artikel</a>
        <a href="about.html">About</a>
        <a href="kontak.html">Contact</a>
      </ul>
    </nav>
```
Kemudian tambahkan css kedalam html
```
*{
    padding: 0;
    margin: 0;
}
/* layout CSS */
#main {
    float: left;
    width: 640px;
    padding: 19px;
}

/* BODY */
body {
    line-height:1;
    font-size:100%;
    font-family:'Open Sans', sans-serif;
    color:#6b6969;
}

/* container */
#container {
    width: 980px;
    height: 2000px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}

/* Header */
header{
    padding: 10px;
    background-color: #ddd8d8;
}
header h1 {
    margin: 20px 10px;
    color: #181616;
}

/* WRAPPER */
#wrapper{
    margin: 0px;
}

/* Navigasi */
nav{
    display: block;
    background-color: rgb(207, 5, 5);
    padding: 5px;
}
ul a{
    color: white;
    display: inline-block;
    padding: 5px;
    margin: 5px;
    text-decoration: none;
}
```
### Hasil
<img width="960" alt="hasil3" src="https://github.com/DimasF3009/Lab4web/assets/115356128/8b04255a-9720-4b46-8b49-bad62e1ac15f">

## Membuat Slide show 
Membuat slideshow dengan html
```
<section id="wrapper">
      <h1 style="margin: 10px 20px;">Indonesia Emas 2045</h1>
      <!-- Slider -->
      <div class="slide">
        <img src="gambar/indonesia1.png" alt="sam1" id="sam1">
        <img src="gambar/indonesia2.jpg" alt="sam2" id="sam2">
        <img src="gambar/indonesia3.jpg" alt="sam3" id="sam3">
      </div>
      <div class="slider-nav">
            <a href="#sam1"></a>
            <a href="#sam2"></a>
            <a href="#sam3"></a>
      </div>
</section>
```
Kemudian tambahkan css kedalam html
```
.slide{
    display: flex;
    aspect-ratio: 16/9;
    overflow-x: auto;
    overflow: hidden;
    scroll-snap-type: x mandatory;
    scroll-behavior: smooth;
}
.slide img{
    max-width: auto;
    padding: 30px;
    flex: 1 0 92%;
    scroll-snap-align: start;
    object-fit: cover;
}
.slider-nav{
    display: flex;
    position: relative;
    column-gap: 5px;
    bottom: 55px;
    left: 150px;
    z-index: 1;
    margin-left:300px;
}
.slider-nav a{
    background-color:grey;
    width:20px;
    height: 20px;
    border-radius: 10px;
    opacity: 0.75;
}
.slider-nav a:hover{
    opacity: 1;
    transition: 1s;
}
```
### Hasil
<img width="595" alt="hasil4" src="https://github.com/DimasF3009/Lab4web/assets/115356128/c50abc80-e67b-4c3a-844c-5e0c4db05800">
<img width="595" alt="hasil5" src="https://github.com/DimasF3009/Lab4web/assets/115356128/21ea9e87-68a4-4df5-b07d-2717cd4ffb2c">
<img width="595" alt="hasil6" src="https://github.com/DimasF3009/Lab4web/assets/115356128/4004a9be-6212-4b4e-a1c2-cd457174bfcd">

## Membuat Sidebar
Membuat sidebar dengan html
```
<section id="wrapper">
      <aside id="sidebar">
          <div class="side-bar">
            <h3 class="title">Other News</h3>
            <ul>
              <li><a href="#">Sport News</a></li>
              <li><a href="#">Political News</a></li>
              <li><a href="#">Economic News</a></li>
              <li><a href="#">Environmental News</a></li>
              <li><a href="#">Domestic News</a></li>
            </ul>
          </div>
          <div class="side-bar">
            <h3 class="title">Widget Text</h3>
            <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt 
              arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer 
              pharetra est nunc, nec pretium nunc pretium ac.</p>
          </div>
      </aside>
</section>
```
Kemudian tambahkan css kedalam html
```
#sidebar{
    float: left;
    width: 260px;
    padding: 20px;
}
.side-bar .title {
    padding:10px 16px;
    background-color:#428bca;
    color:#fff;
}    
.side-bar {
    border:1px solid #eee;
    margin-bottom:20px;
}
.side-bar ul{
    list-style: none; 
}
.side-bar ul li{
   border-bottom:1px solid #eee;
}
.side-bar a{
    padding:10px 16px;
    color:#333;
    display:block;
    text-decoration:none;
}
.side-bar li:hover a {
    background-color:#eee;
}
.side-bar p {
    padding:15px;
    line-height:25px;
}
```
### Hasil
<img width="268" alt="hasil7" src="https://github.com/DimasF3009/Lab4web/assets/115356128/c69a3912-6093-49fa-a6bd-91c090ba1c72">

## Membuat Main content
Membuat main content dengan html
```
<section id="wrapper">
    <section id="main">
        <article class="artikel">
          <p>
            KEMENKO PMK --  Indonesia akan mengalami usia emas pada tahun 2045. Pada saat itu, Indonesia genap berusia 100 tahun alias satu abad. Di masa itu, ditargetkan Indonesia sudah menjadi negara maju dan telah sejajar dengan negara adidaya. 
          </p><br>
          <p>
            Momentum bersejarah tersebut memang masih sekitar saperempat abad lagi. Namun untuk mewujudkannya butuh persiapan yang matang sejak jauh-jauh hari. Sumber daya manusia Indonesia harus unggul, berkualitas, dan memiliki karakter. 
          </p><br>
          <p>
            Menteri Koordinator Bidang Pembangunan Manusia dan Kebudayaan (Menko PMK) Muhadjir Effendy mengatakan, generasi yang akan mewujudkan Indonesia Emas adalah generasi muda, khususnya yang saat ini tengah menempuh pendidikan di perguruan tinggi.
          </p><br>
          <p>
            Dia menerangkan, para mahasiswa/mahasiswi dan lulusan universitas jenjang sarjana saat ini berada di kisaran usia 20 tahun. Menurutnya, pada masa Indonesia berusia 100 tahun yaitu 2045, usia mereka masih sekitar 40 tahun ke atas, yang merupakan usia puncak karir bagi profesional.
          </p><br>
          <p>
            "Artinya, Indonesia Emas itu adalah milik saudara semua, bukan milik saya. Bukan milik mereka yang saat ini usianya sudah di atas 50 tahun," ujar Muhadjir saat menyampaikan sambutan pada Wisuda Ke-105 Periode III Universitas Muhammadiyah Malang (UMM), di UMM Dome Malang, pada Kamis (6/10/2022).
          </p>
        </article>
    </section>
</section>
```
Kemudian tambahkan css kedalam html
```
.artikel{
   margin-left: 10px;
   padding: 30px;
}
.artikel p{
    font-size: 100%;
    justify-content: space-between;
}
```
### Hasi
<img width="833" alt="hasil8" src="https://github.com/DimasF3009/Lab4web/assets/115356128/abeab6ff-8bb5-454e-b63e-75b2fe6675aa">





















