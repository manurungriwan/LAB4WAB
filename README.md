# LAB4WAB
Instruksi Praktikum 4:

1.	Persiapkan text editor misalnya VSCode. 
2.	Buat folder baru dengan nama Lab4Web 
3.	Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya. 
4.	Lakukan validasi dokumen html dengan mengakses http://validator.w3.org  

Langkah-langkah Praktikum 

Persiapan membuat dokumen HTML dengan nama file lab4_box.html seperti berikut. 

<!DOCTYPE html> 
<html lang="en"> 
<head> 
    <meta charset="UTF-8"> 
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
    <title>Box Element</title> 
</head> 
<body> 
    <header> 
        <h1>Box Element</h1> 
    </header> 
</body> 
</html> 
 
Membuat Box Element

Kemudian tambahkan kode untuk membuat box element dengan tag div seperti berikut:

<section> 
    <div class="div1">Div 1</div> 
    <div class="div2">Div 2</div> 
    <div class="div3">Div 3</div>       </section> 
 
CSS Float Property 

Selanjutnya tambahkan deklarasi CSS pada head untuk membuat float element, seperti berikut. 

<style>     div {         float:left;         padding: 10px;  
    }     .div1 { 
        background: red; 
    }     .div2 { 
        background: yellow; 
    }     .div3 { 
        background: green; 
    } 
</style> 
 
Kemudian buka browser untuk melihat hasilnya. 
  
![1 0](https://user-images.githubusercontent.com/56192368/115662844-c8c24300-a369-11eb-968a-33cd94ccdf07.JPG)


Mengatur Clearfix Element 

Clearfix digunakan untuk mengatur element setelah float element. Property clear digunakan untuk mengaturnya. 

Tambahkan element div lainnya seteleah div3 seperti berikut. 

<section> 
    <div class="div1">Div 1</div> 
    <div class="div2">Div 2</div> 
    <div class="div3">Div 3</div>   
    <div class="div4">Div 4</div>     </section> 
 
Kemudian atur property clear pada CSS, seperti berikut. 

.div4 { 
    background-color: blue; 
    clear: left;     float: none; 
} 
 

Selanjutnya buka browser dan refresh kembali. 
  
![1 1](https://user-images.githubusercontent.com/56192368/115662933-e7c0d500-a369-11eb-99a1-a185d9e7b58f.JPG)


Lakukan eksperimen terhadap penggunaan property clear dengan nilai lainnya (left, both, right), dan amati perubahannya.  

Membuat Layout Sederhana 

Buat folder baru dengan nama lab4_layout, kemudian buatlah file baru didalamnya dengan nama home.html, dan file css dengan nama style.css. 

<!DOCTYPE html> 
<html lang="en"> 
<head> 
    <meta charset="UTF-8"> 
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
    <title>Layout Sederhana</title> 
    <link rel="stylesheet" href="style.css"> 
</head> 
<body> 
    <div id="container"> 
         
    </div> 
</body> 
</html> 
 
 
Kemudian tulis kode berikut. 
<header> 
    <h1>Layout Sederhana</h1> 
</header> 
<nav> 
    <a href="home.html" class="active">Home</a> 
    <a href="artikel.html">Artikel</a> 
    <a href="about.html">About</a> 
    <a href="kontak.html">Kontak</a> 
</nav> 
<section id="hero"></section> 
<section id="wrapper"> 
    <section id="main"></section> 
    <aside id="sidebar"></aside> 
</section> 
<footer> 
    <p>&copy; 2021 - Universitas Pelita Bangsa</p> </footer> 


Kemudian buka browser dan lihat hasilnya. 
  
![2 0](https://user-images.githubusercontent.com/56192368/115663165-45552180-a36a-11eb-85e9-0ee064c1f221.JPG)


Kemudian tambahkan kode CSS untuk membuat layoutnya. 

/* import google font */ 
@import 
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400 ;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap'); 
@import 
url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0 ,300;0,700;1,300&display=swap'); 
 
/* Reset CSS */ 
* {     margin: 0;     padding: 0; 
}  body { 
    line-height:1;     font-size:100%; 
    font-family:'Open Sans', sans-serif;     color:#5a5a5a; 
} 
 
#container {     width: 980px;     margin: 0 auto; 
    box-shadow: 0 0 1em #cccccc; 
} 
 
/* header */ header { 
    padding: 20px; 
}  
header h1 { 
    margin: 20px 10px;     color: #b5b5b5; 
} 
 
Kemudian lihat hasilnya pada browser. 
  

![2 1](https://user-images.githubusercontent.com/56192368/115663202-5c940f00-a36a-11eb-822b-2aab927b206e.JPG)


Membuat Navigasi 
Kemudian selanjutnya mengatur navigasi. 

/* navigasi */ nav { 
    display: block; 
    background-color: #1f5faa; 
}  nav a { 
    padding: 15px 30px;     display: inline-block;     color: #ffffff;     font-size: 14px;     text-decoration: none;     font-weight: bold; 
}  nav a.active, nav a:hover { 
    background-color: #2b83ea; } 
 
Kemudian lihat hasilnya. 
  
![3 0](https://user-images.githubusercontent.com/56192368/115663239-6d448500-a36a-11eb-9f1c-230908bae52d.JPG)
  

Membuat Hero Panel: 

Selanjutnya membuat hero panel. Tambahkan kode HTML dan CSS seperti berikut:

<section id="hero"> 
    <h1>Hello World!</h1> 
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p> 
    <a href="home.html" class="btn btn-large">Learn more &raquo;</a> </section> 
 
/* Hero Panel */ #hero { 
    background-color: #e4e4e5;     padding: 50px 20px;     margin-bottom: 20px; 
} 
 #hero h1 {     margin-bottom: 20px;     font-size: 35px; 
} 
 #hero p { 
    margin-bottom: 20px;     font-size: 18px;     line-height: 25px; 
} 
 
  
![3 1](https://user-images.githubusercontent.com/56192368/115663336-8fd69e00-a36a-11eb-8c9e-a71cc93cd833.JPG)


Mengatur Layout Main dan Sidebar:

Selanjutnya mengatur main content dan sidebar, tambahkan CSS float:

/* main content */ 
#wrapper {     margin: 0; } 
 #main {     float: left;     width: 640px;     padding: 20px; 
} 
 
/* sidebar area */ 
#sidebar {     float: left;     width: 260px;     padding: 20px; 
} 
 
Membuat Sidebar Widget 

Kemudian selanjutnya menambahkan element lain dalam sidebar.  

<aside id="sidebar"> 
    <div class="widget-box"> 
        <h3 class="title">Widget Header</h3> 
        <ul> 
            <li><a href="#">Widget Link</a></li> 
            <li><a href="#">Widget Link</a></li> 
            <li><a href="#">Widget Link</a></li> 
            <li><a href="#">Widget Link</a></li> 
            <li><a href="#">Widget Link</a></li> 
        </ul> 
    </div> 
    <div class="widget-box"> 
        <h3 class="title">Widget Text</h3> 
        <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p> 
    </div> 
</aside> 
 
Kemudian tambahkan CSS:

/* widget */ .widget-box { 
    border:1px solid #eee;     margin-bottom:20px; 
} 
 
.widget-box  .title {     padding:10px 16px;     background-color:#428bca;     color:#fff; 
} 
 
.widget-box ul { 
    list-style-type:none; 
} 
 
.widget-box li { 
    border-bottom:1px solid #eee;
    
    

![4 0](https://user-images.githubusercontent.com/56192368/115663721-1e4b1f80-a36b-11eb-8b2b-ac26bbc6b5bd.JPG)

 
Mengatur Footer:

Selanjutnya mengatur tampilan footer. Tambahkan CSS untuk footer. 

/* footer */ footer {     clear:both; 
    background-color:#1d1d1d;     padding:20px;     color:#eee; 
} 


![4 1](https://user-images.githubusercontent.com/56192368/115663756-2c00a500-a36b-11eb-9f8f-3bd51d3f361f.JPG)


Menambahkan Elemen lainnya pada Main Content 
 
<section id="main"> 
    <div class="row"> 
        <div class="box"> 
            <img src="https://dummyimage.com/120/db7d25/fff.png" alt="" class="image-circle">             <h3>Heading</h3> 
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p> 
            <a href="#" class="btn btn-default">View detail</a> 
        </div> 
        <div class="box"> 
            <img src="https://dummyimage.com/120/3e73e6/fff.png" alt="" class="image-circle">             <h3>Heading</h3> 
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p> 
            <a href="#" class="btn btn-default">View detail</a> 
        </div> 
        <div class="box"> 
            <img src="https://dummyimage.com/120/71e6d4/fff.png" alt="" class="image-circle">             <h3>Heading</h3> 
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p> 
            <a href="#" class="btn btn-default">View detail</a> 
        </div> 
    </div> 
</section> 
 
Kemudian tambahkan CSS:

/* box */ .box { 
    display:block;     float:left;     width:33.333333%;     box-sizing:border-box;     -moz-box-sizing:border-box; 
    -webkit-box-sizing:border-box; 

Lihat hasilnya dibrowser. 

![5 0](https://user-images.githubusercontent.com/56192368/115663830-45a1ec80-a36b-11eb-9aaa-71fbb9363d03.JPG)


Menambahkan Content Artikel 

Selanjutnya membuat content artikel. Tambahkan HTML berikut pada main content. 

<hr class="divider" /> 
<article class="entry"> 
    <h2>First featurette heading.</h2> 
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt=""> 
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p> 
</article> 
<hr class="divider" /> 
<article class="entry"> 
    <h2>First featurette heading.</h2> 
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" class="right-img"> 
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p> 
</article> 
 

Kemudian tambahkan CSS:

.divider {     border:0; 
    border-top:1px solid #eeeeee;     margin:40px 0; 
} 
 
/* entry */ .entry { 
    margin: 15px 0; 
} 
 
.entry h2 { 
    margin-bottom: 20px; 

![TERAHIR](https://user-images.githubusercontent.com/56192368/115663926-6407e800-a36b-11eb-8e29-c36dd66f99ef.JPG)



Pertanyaan dan Tugas:

1. Tambahkan Layout untuk menu About
=> buat single layout yang berisi deskripsi, portfolio, dll
JAWABAN:

![ABOUT](https://user-images.githubusercontent.com/56192368/115664803-877f6280-a36c-11eb-9e64-d8c5fa23e9e5.JPG)

2. Tambahkan layout untuk menu Contact
=> yang berisi form isian: nama, email, message, dll
JAWABAN:

![CANTACT PERSON](https://user-images.githubusercontent.com/56192368/115664857-9f56e680-a36c-11eb-8871-d471a5e107cc.JPG)


SEKIAN DAN TERIMAKASIH SELAMAT MENUNAIKAN IBADAH PUASA 

                        &
              
            MOHON MAAF LAHIR DAN BATIN
            
