<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>ARKFLIX</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial,Helvetica,sans-serif;
}

body{
    background:#080808;
    color:white;
    overflow-x:hidden;
}

/* NAVBAR */

.navbar{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    height:65px;
    padding:0 20px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    background:linear-gradient(
        to bottom,
        rgba(0,0,0,.95),
        rgba(0,0,0,.2)
    );
    z-index:100;
}

.logo{
    font-size:25px;
    font-weight:900;
    letter-spacing:-1px;
}

.logo span{
    color:#e50914;
}

.nav-icons{
    display:flex;
    gap:18px;
    font-size:22px;
}

/* HERO */

.hero{
    height:570px;
    position:relative;
    display:flex;
    align-items:flex-end;
    padding:0 20px 55px;
    background:
    linear-gradient(to top,#080808 5%,transparent 55%),
    linear-gradient(to right,rgba(0,0,0,.9),transparent 70%),
    url("https://images.unsplash.com/photo-1489599849927-2ee91cede3ba?auto=format&fit=crop&w=1400&q=80")
    center/cover;
}

.hero-content{
    max-width:340px;
}

.badge{
    color:#e50914;
    font-weight:bold;
    letter-spacing:2px;
    margin-bottom:10px;
}

.hero h1{
    font-size:42px;
    line-height:1;
    margin-bottom:12px;
}

.hero p{
    color:#ddd;
    font-size:14px;
    line-height:1.5;
    margin-bottom:18px;
}

.buttons{
    display:flex;
    gap:10px;
}

button{
    border:0;
    border-radius:5px;
    padding:11px 20px;
    font-size:14px;
    font-weight:bold;
}

.play{
    background:white;
    color:black;
}

.info{
    background:#555b;
    color:white;
}

/* SECTIONS */

.section{
    padding:15px 20px 5px;
}

.section h2{
    font-size:19px;
    margin-bottom:13px;
}

.row{
    display:flex;
    gap:10px;
    overflow-x:auto;
    scrollbar-width:none;
}

.row::-webkit-scrollbar{
    display:none;
}

/* MOVIE CARD */

.card{
    min-width:125px;
    height:185px;
    border-radius:7px;
    overflow:hidden;
    position:relative;
    background:#181818;
    transition:.25s;
}

.card img{
    width:100%;
    height:100%;
    object-fit:cover;
}

.card:hover{
    transform:scale(1.05);
}

.card-title{
    position:absolute;
    bottom:0;
    width:100%;
    padding:25px 7px 7px;
    background:linear-gradient(transparent,rgba(0,0,0,.95));
    font-size:12px;
    font-weight:bold;
}

/* CONTINUE WATCHING */

.progress{
    position:absolute;
    bottom:0;
    left:0;
    height:4px;
    background:#e50914;
}

/* BOTTOM NAV */

.bottom-nav{
    position:fixed;
    bottom:0;
    left:0;
    width:100%;
    height:65px;
    background:#090909;
    border-top:1px solid #222;
    display:flex;
    justify-content:space-around;
    align-items:center;
    z-index:100;
}

.nav-item{
    text-align:center;
    color:#888;
    font-size:11px;
}

.nav-item div{
    font-size:21px;
    margin-bottom:3px;
}

.active{
    color:white;
}

@media(min-width:700px){

    .card{
        min-width:170px;
        height:250px;
    }

    .hero{
        height:650px;
    }

    .hero h1{
        font-size:55px;
    }
}
</style>
</head>

<body>

<!-- NAVBAR -->

<header class="navbar">

    <div class="logo">
        ARK<span>FLIX</span>
    </div>

    <div class="nav-icons">
        🔍
        👤
    </div>

</header>


<!-- HERO -->

<section class="hero">

    <div class="hero-content">

        <div class="badge">ARKFLIX ORIGINAL</div>

        <h1>THE LAST JOURNEY</h1>

        <p>
            A mysterious journey begins when a forgotten secret
            changes everything.
        </p>

        <div class="buttons">

            <button class="play">
                ▶ Play
            </button>

            <button class="info">
                ⓘ More Info
            </button>

        </div>

    </div>

</section>


<!-- TRENDING -->

<section class="section">

<h2>🔥 Trending Now</h2>

<div class="row">

<div class="card">
<img src="https://images.unsplash.com/photo-1485846234645-a62644f84728?auto=format&fit=crop&w=500&q=80">
<div class="card-title">The Mystery</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1489599849927-2ee91cede3ba?auto=format&fit=crop&w=500&q=80">
<div class="card-title">Dark Night</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1500534623283-312aade485b7?auto=format&fit=crop&w=500&q=80">
<div class="card-title">Lost World</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1536440136628-849c177e76a1?auto=format&fit=crop&w=500&q=80">
<div class="card-title">Final Hour</div>
</div>

</div>

</section>


<!-- CONTINUE WATCHING -->

<section class="section">

<h2>▶ Continue Watching</h2>

<div class="row">

<div class="card">

<img src="https://images.unsplash.com/photo-1516035069371-29a1b244cc32?auto=format&fit=crop&w=500&q=80">

<div class="card-title">
Episode 3
</div>

<div class="progress" style="width:65%;"></div>

</div>


<div class="card">

<img src="https://images.unsplash.com/photo-1517604931442-7e0c8ed2963c?auto=format&fit=crop&w=500&q=80">

<div class="card-title">
Episode 5
</div>

<div class="progress" style="width:35%;"></div>

</div>

</div>

</section>


<!-- POPULAR -->

<section class="section">

<h2>⭐ Popular Movies</h2>

<div class="row">

<div class="card">
<img src="https://images.unsplash.com/photo-1574267432553-4b4628081c31?auto=format&fit=crop&w=500&q=80">
<div class="card-title">The Warrior</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1598899134739-24c46f58b8c0?auto=format&fit=crop&w=500&q=80">
<div class="card-title">Night City</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1440404653325-ab127d49abc1?auto=format&fit=crop&w=500&q=80">
<div class="card-title">The Story</div>
</div>

</div>

</section>


<!-- BOTTOM NAV -->

<nav class="bottom-nav">

<div class="nav-item active">
<div>⌂</div>
Home
</div>

<div class="nav-item">
<div>🔍</div>
Search
</div>

<div class="nav-item">
<div>＋</div>
My List
</div>

<div class="nav-item">
<div>⬇</div>
Downloads
</div>

<div class="nav-item">
<div>👤</div>
Profile
</div>

</nav>

</body>
</html>
