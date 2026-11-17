<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Website Makanan</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#fff5eb;
    overflow-x:hidden;
}

/* TEAM */
.team{
    position:fixed;
    top:15px;
    right:15px;
    z-index:999;
    background:rgba(0,0,0,0.5);
    padding:12px 18px;
    border-radius:15px;
    color:white;
    backdrop-filter:blur(5px);
}

.team h3{
    margin-bottom:8px;
    font-size:18px;
}

.team p{
    line-height:24px;
}

/* RGB */
.rgb{
    background:linear-gradient(
        90deg,
        red,
        orange,
        yellow,
        lime,
        cyan,
        blue,
        violet,
        red
    );

    background-size:400%;
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;

    animation:rgb 5s linear infinite;
    font-weight:bold;
}

@keyframes rgb{
    0%{
        background-position:0%;
    }

    100%{
        background-position:400%;
    }
}

/* WELCOME */
#welcome{
    width:100%;
    height:100vh;
    background:linear-gradient(135deg,#ff9800,#ff5722);
    display:flex;
    justify-content:center;
    align-items:center;
    flex-direction:column;
    color:white;
    text-align:center;
}

#welcome h1{
    font-size:70px;
    text-shadow:0 0 20px rgba(255,255,255,0.7);
    animation:zoom 2s infinite alternate;
}

#welcome h2{
    margin-top:15px;
    font-size:30px;
}

#welcome p{
    margin-top:10px;
    font-size:20px;
}

@keyframes zoom{
    from{
        transform:scale(1);
    }

    to{
        transform:scale(1.08);
    }
}

/* BUTTON */
.btn{
    margin-top:35px;
    padding:15px 45px;
    border:none;
    border-radius:40px;
    background:white;
    color:#ff5722;
    font-size:20px;
    font-weight:bold;
    cursor:pointer;
    transition:0.3s;
}

.btn:hover{
    transform:scale(1.1);
    background:#ffe0b2;
}

/* MENU */
#menu{
    display:none;
    padding:40px;
}

.title{
    text-align:center;
    font-size:50px;
    margin-bottom:40px;
    color:#ff5722;
}

.food-container{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
    gap:30px;
}

.food-card{
    background:white;
    border-radius:20px;
    overflow:hidden;
    box-shadow:0 5px 15px rgba(0,0,0,0.2);
    transition:0.3s;
    cursor:pointer;
}

.food-card:hover{
    transform:translateY(-10px) scale(1.03);
}

.food-card img{
    width:100%;
    height:220px;
    object-fit:cover;
}

.food-info{
    padding:20px;
}

.food-info h2{
    color:#ff5722;
    margin-bottom:10px;
}

/* POPUP */
.popup{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    height:100%;
    background:rgba(0,0,0,0.7);
    display:none;
    justify-content:center;
    align-items:center;
    padding:20px;
    z-index:9999;
}

.popup-content{
    background:white;
    width:90%;
    max-width:550px;
    border-radius:20px;
    overflow:hidden;
    animation:popup 0.3s;
}

.popup-content img{
    width:100%;
    height:300px;
    object-fit:cover;
}

.popup-text{
    padding:20px;
}

.popup-text h2{
    color:#ff5722;
    margin-bottom:15px;
}

.close{
    margin-top:15px;
    padding:12px 20px;
    border:none;
    border-radius:10px;
    background:#ff5722;
    color:white;
    cursor:pointer;
}

@keyframes popup{
    from{
        transform:scale(0.7);
        opacity:0;
    }

    to{
        transform:scale(1);
        opacity:1;
    }
}

</style>
</head>
<body>

<!-- AUDIO -->
<audio id="klikSound">
    <source src="https://www.image2url.com/r2/default/audio/1778759222931-e5b62562-fdfe-41f5-b06f-5826470e4b53.mp3" type="audio/mpeg">
</audio>

<!-- TEAM -->
<div class="team">
    <h3>👑 Team</h3>

    <p class="rgb">Adil Putra</p>
    <p class="rgb">Aji Rafa</p>
    <p class="rgb">Bayi Aji</p>
    <p class="rgb">Medi Putro</p>
</div>

<!-- WELCOME -->
<section id="welcome">

    <h1>WELCOME</h1>

    <h2 class="rgb">
        Adil Putra
    </h2>

    <p>
        Selamat Datang di Website Makanan 🍔🍕🍟🍎
    </p>

    <button class="btn" onclick="masukMenu()">
        Masuk
    </button>

</section>

<!-- MENU -->
<section id="menu">

    <h1 class="title">
        🍽️ Menu Makanan Lengkap
    </h1>

    <div class="food-container">

        <!-- BURGER -->
        <div class="food-card"
        onclick="showPopup(
        'Burger',
        'https://images.unsplash.com/photo-1568901346375-23c9450c58cd?q=80&w=1200&auto=format&fit=crop',
        'Burger adalah makanan cepat saji berisi daging, sayur, dan saus yang lezat.'
        )">

            <img src="https://images.unsplash.com/photo-1568901346375-23c9450c58cd?q=80&w=1200&auto=format&fit=crop">

            <div class="food-info">
                <h2>Burger 🍔</h2>
                <p>Klik untuk penjelasan</p>
            </div>
        </div>

        <!-- PIZZA -->
        <div class="food-card"
        onclick="showPopup(
        'Pizza',
        'https://images.unsplash.com/photo-1513104890138-7c749659a591?q=80&w=1200&auto=format&fit=crop',
        'Pizza adalah makanan khas Italia dengan topping keju dan saus tomat.'
        )">

            <img src="https://images.unsplash.com/photo-1513104890138-7c749659a591?q=80&w=1200&auto=format&fit=crop">

            <div class="food-info">
                <h2>Pizza 🍕</h2>
                <p>Klik untuk penjelasan</p>
            </div>
        </div>

        <!-- SUSHI -->
        <div class="food-card"
        onclick="showPopup(
        'Sushi',
        'https://images.unsplash.com/photo-1579871494447-9811cf80d66c?q=80&w=1200&auto=format&fit=crop',
        'Sushi adalah makanan Jepang yang dibuat dari nasi dan ikan segar.'
        )">

            <img src="https://images.unsplash.com/photo-1579871494447-9811cf80d66c?q=80&w=1200&auto=format&fit=crop">

            <div class="food-info">
                <h2>Sushi 🍣</h2>
                <p>Klik untuk penjelasan</p>
            </div>
        </div>

        <!-- ES KRIM -->
        <div class="food-card"
        onclick="showPopup(
        'Es Krim',
        'https://images.unsplash.com/photo-1563805042-7684c019e1cb?q=80&w=1200&auto=format&fit=crop',
        'Es krim adalah makanan manis dan dingin yang cocok dimakan saat cuaca panas.'
        )">

            <img src="https://images.unsplash.com/photo-1563805042-7684c019e1cb?q=80&w=1200&auto=format&fit=crop">

            <div class="food-info">
                <h2>Es Krim 🍦</h2>
                <p>Klik untuk penjelasan</p>
            </div>
        </div>

        <!-- BUAH -->
        <div class="food-card"
        onclick="showPopup(
        'Buah-buahan',
        'https://images.unsplash.com/photo-1619566636858-adf3ef46400b?q=80&w=1200&auto=format&fit=crop',
        'Buah sangat sehat karena kaya vitamin dan nutrisi.'
        )">

            <img src="https://images.unsplash.com/photo-1619566636858-adf3ef46400b?q=80&w=1200&auto=format&fit=crop">

            <div class="food-info">
                <h2>Buah 🍎</h2>
                <p>Klik untuk penjelasan</p>
            </div>
        </div>

        <!-- MIE -->
        <div class="food-card"
        onclick="showPopup(
        'Mie',
        'https://images.unsplash.com/photo-1612929633738-8fe44f7ec841?q=80&w=1200&auto=format&fit=crop',
        'Mie adalah makanan favorit banyak orang dengan rasa gurih dan nikmat.'
        )">

            <img src="https://images.unsplash.com/photo-1612929633738-8fe44f7ec841?q=80&w=1200&auto=format&fit=crop">

            <div class="food-info">
                <h2>Mie 🍜</h2>
                <p>Klik untuk penjelasan</p>
            </div>
        </div>

        <!-- AYAM -->
        <div class="food-card"
        onclick="showPopup(
        'Ayam Goreng',
        'https://images.unsplash.com/photo-1562967916-eb82221dfb92?q=80&w=1200&auto=format&fit=crop',
        'Ayam goreng memiliki rasa renyah dan gurih yang disukai banyak orang.'
        )">

            <img src="https://images.unsplash.com/photo-1562967916-eb82221dfb92?q=80&w=1200&auto=format&fit=crop">

            <div class="food-info">
                <h2>Ayam Goreng 🍗</h2>
                <p>Klik untuk penjelasan</p>
            </div>
        </div>

        <!-- DONAT -->
        <div class="food-card"
        onclick="showPopup(
        'Donat',
        'https://images.unsplash.com/photo-1551024601-bec78aea704b?q=80&w=1200&auto=format&fit=crop',
        'Donat adalah makanan manis berbentuk lingkaran dengan topping menarik.'
        )">

            <img src="https://images.unsplash.com/photo-1551024601-bec78aea704b?q=80&w=1200&auto=format&fit=crop">

            <div class="food-info">
                <h2>Donat 🍩</h2>
                <p>Klik untuk penjelasan</p>
            </div>
        </div>

        <!-- KOPI -->
        <div class="food-card"
        onclick="showPopup(
        'Kopi',
        'https://images.unsplash.com/photo-1495474472287-4d71bcdd2085?q=80&w=1200&auto=format&fit=crop',
        'Kopi adalah minuman favorit yang dapat membuat tubuh lebih segar.'
        )">

            <img src="https://images.unsplash.com/photo-1495474472287-4d71bcdd2085?q=80&w=1200&auto=format&fit=crop">

            <div class="food-info">
                <h2>Kopi ☕</h2>
                <p>Klik untuk penjelasan</p>
            </div>
        </div>

        <!-- SALAD -->
        <div class="food-card"
        onclick="showPopup(
        'Salad',
        'https://images.unsplash.com/photo-1546793665-c74683f339c1?q=80&w=1200&auto=format&fit=crop',
        'Salad adalah makanan sehat berisi sayur dan buah segar.'
        )">

            <img src="https://images.unsplash.com/photo-1546793665-c74683f339c1?q=80&w=1200&auto=format&fit=crop">

            <div class="food-info">
                <h2>Salad 🥗</h2>
                <p>Klik untuk penjelasan</p>
            </div>
        </div>

    </div>

</section>

<!-- POPUP -->
<div class="popup" id="popup">

    <div class="popup-content">

        <img id="popup-img">

        <div class="popup-text">

            <h2 id="popup-title"></h2>

            <p id="popup-desc"></p>

            <button class="close" onclick="closePopup()">
                Tutup
            </button>

        </div>

    </div>

</div>

<script>

function masukMenu(){

    // PLAY AUDIO
    document.getElementById("klikSound").play();

    // MASUK MENU
    setTimeout(() => {

        document.getElementById("welcome").style.display="none";

        document.getElementById("menu").style.display="block";

    }, 500);
}

function showPopup(title,img,desc){

    document.getElementById("popup").style.display="flex";

    document.getElementById("popup-title").innerText=title;

    document.getElementById("popup-img").src=img;

    document.getElementById("popup-desc").innerText=desc;
}

function closePopup(){

    document.getElementById("popup").style.display="none";
}

</script>

</body>
  </html>
