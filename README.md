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
<img width="960" alt="hasil3" src="https://github.com/DimasF3009/Lab4web/assets/115356128/8b04255a-9720-4b46-8b49-bad62e1ac15f">


