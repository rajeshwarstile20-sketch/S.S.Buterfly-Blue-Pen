<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>S.S Butterfly Blue Pen | Premium Writing</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial,Helvetica,sans-serif;
}

:root{
    --blue:#087cff;
    --dark:#06111f;
    --light:#eef7ff;
    --cyan:#20d9ff;
    --silver:#dce5ee;
}

body{
    min-height:100vh;
    background:
        radial-gradient(circle at 20% 20%,rgba(0,140,255,.18),transparent 30%),
        radial-gradient(circle at 80% 80%,rgba(0,210,255,.12),transparent 30%),
        linear-gradient(135deg,#020812,#081827 55%,#03101d);
    color:white;
    overflow-x:hidden;
}

/* Background particles */
.particle{
    position:fixed;
    width:4px;
    height:4px;
    background:#54cfff;
    border-radius:50%;
    opacity:.5;
    animation:float 8s infinite ease-in-out;
    pointer-events:none;
}

.p1{left:8%;top:20%;animation-delay:0s}
.p2{left:18%;top:70%;animation-delay:2s}
.p3{left:75%;top:18%;animation-delay:1s}
.p4{left:90%;top:60%;animation-delay:3s}
.p5{left:55%;top:85%;animation-delay:4s}

@keyframes float{
    0%,100%{transform:translateY(0) scale(1)}
    50%{transform:translateY(-70px) scale(1.7)}
}

/* Navigation */
nav{
    height:75px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:0 7%;
    border-bottom:1px solid rgba(255,255,255,.08);
    backdrop-filter:blur(15px);
    position:relative;
    z-index:10;
}

.logo{
    font-size:24px;
    font-weight:800;
    letter-spacing:1px;
}

.logo span{
    color:var(--cyan);
}

.nav-btn{
    padding:11px 22px;
    border:1px solid rgba(255,255,255,.25);
    border-radius:30px;
    color:white;
    background:rgba(255,255,255,.05);
    cursor:pointer;
    transition:.3s;
}

.nav-btn:hover{
    background:var(--blue);
    transform:translateY(-2px);
    box-shadow:0 8px 25px rgba(0,130,255,.4);
}

/* Hero */
.hero{
    max-width:1250px;
    margin:auto;
    min-height:calc(100vh - 75px);
    display:grid;
    grid-template-columns:1fr 1fr;
    align-items:center;
    gap:40px;
    padding:60px 30px;
}

.badge{
    display:inline-block;
    padding:8px 15px;
    border:1px solid rgba(60,190,255,.4);
    background:rgba(0,130,255,.08);
    border-radius:50px;
    color:#66d7ff;
    font-size:13px;
    margin-bottom:20px;
}

h1{
    font-size:clamp(45px,6vw,78px);
    line-height:.95;
    letter-spacing:-3px;
    margin-bottom:22px;
}

h1 span{
    color:var(--blue);
    text-shadow:0 0 35px rgba(0,130,255,.5);
}

.description{
    max-width:570px;
    color:#a9bacb;
    line-height:1.8;
    font-size:17px;
    margin-bottom:28px;
}

.price{
    font-size:36px;
    font-weight:800;
    margin-bottom:22px;
}

.price small{
    color:#8b9aaa;
    text-decoration:line-through;
    font-size:18px;
    margin-left:10px;
}

.buttons{
    display:flex;
    gap:15px;
    flex-wrap:wrap;
}

.btn{
    border:0;
    padding:15px 27px;
    border-radius:12px;
    font-weight:700;
    font-size:15px;
    cursor:pointer;
    transition:.35s;
}

.primary{
    background:linear-gradient(135deg,#0088ff,#0055e8);
    color:white;
    box-shadow:0 12px 30px rgba(0,100,255,.35);
}

.primary:hover{
    transform:translateY(-5px) scale(1.03);
    box-shadow:0 18px 40px rgba(0,120,255,.55);
}

.secondary{
    background:rgba(255,255,255,.07);
    color:white;
    border:1px solid rgba(255,255,255,.16);
}

.secondary:hover{
    background:rgba(255,255,255,.13);
}

/* Product stage */
.product-stage{
    height:570px;
    display:flex;
    justify-content:center;
    align-items:center;
    perspective:1200px;
    position:relative;
}

.glow{
    position:absolute;
    width:330px;
    height:330px;
    border-radius:50%;
    background:rgba(0,145,255,.23);
    filter:blur(55px);
    animation:pulse 4s infinite;
}

@keyframes pulse{
    0%,100%{transform:scale(.9);opacity:.55}
    50%{transform:scale(1.15);opacity:.85}
}

/* Pen */
.pen{
    width:460px;
    height:95px;
    position:relative;
    transform-style:preserve-3d;
    transform:rotate(-20deg) rotateY(-20deg);
    animation:penFloat 5s ease-in-out infinite;
    filter:drop-shadow(0 35px 20px rgba(0,0,0,.6));
    cursor:pointer;
}

@keyframes penFloat{
    0%,100%{
        transform:rotate(-20deg) rotateY(-20deg) translateY(0);
    }
    50%{
        transform:rotate(-18deg) rotateY(-10deg) translateY(-18px);
    }
}

/* Main barrel */
.barrel{
    position:absolute;
    left:35px;
    top:22px;
    width:330px;
    height:50px;
    border-radius:25px;
    background:
        linear-gradient(
            180deg,
            #bfeeff 0%,
            #168eff 17%,
            #0055c8 48%,
            #003a91 70%,
            #4bbaff 100%
        );
    box-shadow:
        inset 0 6px 8px rgba(255,255,255,.45),
        inset 0 -8px 10px rgba(0,0,0,.4),
        0 5px 15px rgba(0,0,0,.5);
}

/* Highlight */
.barrel:before{
    content:"";
    position:absolute;
    top:8px;
    left:18px;
    width:270px;
    height:7px;
    border-radius:10px;
    background:rgba(255,255,255,.55);
    filter:blur(2px);
}

/* Pen grip */
.grip{
    position:absolute;
    left:345px;
    top:27px;
    width:70px;
    height:40px;
    border-radius:8px 20px 20px 8px;
    background:linear-gradient(
        180deg,
        #f5fbff,
        #8f9aa5 45%,
        #f7ffff 70%,
        #6c7781
    );
    box-shadow:inset 0 3px 4px white;
}

/* Tip */
.tip{
    position:absolute;
    left:405px;
    top:35px;
    width:70px;
    height:25px;
    background:linear-gradient(90deg,#b7c1c9,#fff,#69747d);
    clip-path:polygon(0 0,100% 50%,0 100%);
    filter:drop-shadow(4px 5px 5px rgba(0,0,0,.5));
}

.tip:after{
    content:"";
    position:absolute;
    right:0;
    top:9px;
    width:15px;
    height:7px;
    background:#202a32;
    border-radius:50%;
}

/* Rear cap */
.cap{
    position:absolute;
    left:5px;
    top:20px;
    width:45px;
    height:55px;
    border-radius:20px 7px 7px 20px;
    background:linear-gradient(
        90deg,
        #59636c,
        #eaf1f5,
        #707a84
    );
}

/* Butterfly logo */
.butterfly{
    position:absolute;
    left:155px;
    top:5px;
    width:65px;
    height:40px;
}

.wing{
    position:absolute;
    width:27px;
    height:34px;
    background:linear-gradient(135deg,#dff8ff,#ffffff,#9bdfff);
    border:1px solid rgba(0,70,150,.5);
    box-shadow:0 2px 5px rgba(0,0,0,.3);
}

.wing.left{
    left:3px;
    top:3px;
    border-radius:80% 20% 60% 40%;
    transform:rotate(-25deg);
}

.wing.right{
    right:3px;
    top:3px;
    border-radius:20% 80% 40% 60%;
    transform:rotate(25deg);
}

.butterfly .body{
    position:absolute;
    left:30px;
    top:5px;
    width:5px;
    height:30px;
    border-radius:5px;
    background:#1c2730;
}

/* Clip */
.clip{
    position:absolute;
    left:15px;
    top:5px;
    width:105px;
    height:10px;
    border-radius:10px;
    background:linear-gradient(90deg,#68737c,#ffffff,#89939c);
    box-shadow:0 2px 3px rgba(0,0,0,.5);
}

.clip:after{
    content:"";
    position:absolute;
    left:8px;
    top:5px;
    width:80px;
    height:30px;
    border-left:5px solid #aeb9c2;
    border-radius:20px;
}

/* Features */
.features{
    display:flex;
    gap:12px;
    margin-top:30px;
    flex-wrap:wrap;
}

.feature{
    padding:10px 15px;
    background:rgba(255,255,255,.05);
    border:1px solid rgba(255,255,255,.08);
    border-radius:10px;
    color:#b9c8d6;
    font-size:13px;
}

/* Product cards */
.info{
    max-width:1200px;
    margin:0 auto 70px;
    padding:0 30px;
}

.info-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:20px;
}

.card{
    padding:28px;
    border-radius:20px;
    background:linear-gradient(
        145deg,
        rgba(255,255,255,.08),
        rgba(255,255,255,.025)
    );
    border:1px solid rgba(255,255,255,.1);
    backdrop-filter:blur(15px);
    transition:.4s;
}

.card:hover{
    transform:translateY(-10px) rotateX(3deg);
    border-color:rgba(40,170,255,.4);
    box-shadow:0 20px 50px rgba(0,100,255,.12);
}

.card-icon{
    font-size:32px;
    margin-bottom:15px;
}

.card h3{
    margin-bottom:10px;
}

.card p{
    color:#91a5b8;
    line-height:1.6;
    font-size:14px;
}

/* Modal */
.modal{
    position:fixed;
    inset:0;
    background:rgba(0,0,0,.75);
    display:none;
    align-items:center;
    justify-content:center;
    z-index:100;
    backdrop-filter:blur(8px);
}

.modal-box{
    width:min(450px,90%);
    padding:35px;
    border-radius:25px;
    background:#0b1b2b;
    border:1px solid rgba(255,255,255,.15);
    box-shadow:0 30px 80px rgba(0,0,0,.6);
    text-align:center;
    animation:modalIn .4s ease;
}

@keyframes modalIn{
    from{transform:scale(.8);opacity:0}
    to{transform:scale(1);opacity:1}
}

.modal-box h2{
    margin-bottom:15px;
}

.modal-box p{
    color:#9db0c1;
    line-height:1.6;
    margin-bottom:20px;
}

.close{
    background:#168cff;
    color:white;
    border:0;
    padding:12px 25px;
    border-radius:10px;
    cursor:pointer;
}

/* Responsive */
@media(max-width:850px){
    .hero{
        grid-template-columns:1fr;
        text-align:center;
    }

    .description{
        margin-left:auto;
        margin-right:auto;
    }

    .buttons,.features{
        justify-content:center;
    }

    .product-stage{
        height:430px;
        transform:scale(.8);
    }

    .info-grid{
        grid-template-columns:1fr;
    }
}

@media(max-width:500px){
    nav{
        padding:0 20px;
    }

    .hero{
        padding:40px 18px;
    }

    h1{
        font-size:50px;
    }

    .product-stage{
        transform:scale(.62);
        margin-top:-30px;
    }
}
</style>
</head>

<body>

<div class="particle p1"></div>
<div class="particle p2"></div>
<div class="particle p3"></div>
<div class="particle p4"></div>
<div class="particle p5"></div>

<nav>
    <div class="logo">S.S <span>BUTTERFLY</span></div>
    <button class="nav-btn" onclick="openModal()">Buy Now</button>
</nav>

<main class="hero">

    <section>
        <div class="badge">✦ PREMIUM BLUE EDITION</div>

        <h1>
            Write With<br>
            <span>Confidence.</span>
        </h1>

        <p class="description">
            Meet the S.S Butterfly Blue Pen — a sleek combination of
            elegant design, smooth writing performance and a premium
            metallic-inspired finish made for everyday writing.
        </p>

        <div class="price">
            ₹149
            <small>₹199</small>
        </div>

        <div class="buttons">
            <button class="btn primary" onclick="openModal()">
                🛒 Buy S.S Butterfly
            </button>

            <button class="btn secondary" onclick="showDetails()">
                View Features
            </button>
        </div>

        <div class="features">
            <div class="feature">✓ Smooth Writing</div>
            <div class="feature">✓ Premium Finish</div>
            <div class="feature">✓ Comfortable Grip</div>
        </div>
    </section>


    <!-- 3D PRODUCT -->
    <section class="product-stage" id="productStage">

        <div class="glow"></div>

        <div class="pen" id="pen">

            <div class="clip"></div>

            <div class="cap"></div>

            <div class="barrel">

                <div class="butterfly">
                    <div class="wing left"></div>
                    <div class="wing right"></div>
                    <div class="body"></div>
                </div>

            </div>

            <div class="grip"></div>

            <div class="tip"></div>

        </div>
    </section>

</main>


<section class="info" id="details">

    <div class="info-grid">

        <div class="card">
            <div class="card-icon">🖊️</div>
            <h3>Ultra Smooth Writing</h3>
            <p>
                Designed for comfortable everyday writing with a
                smooth-flowing blue ink experience.
            </p>
        </div>

        <div class="card">
            <div class="card-icon">💎</div>
            <h3>Premium Design</h3>
            <p>
                A stylish blue body with metallic-inspired detailing
                gives the pen a sophisticated appearance.
            </p>
        </div>

        <div class="card">
            <div class="card-icon">🦋</div>
            <h3>Butterfly Identity</h3>
            <p>
                The signature butterfly-inspired detailing creates a
                distinctive visual identity for the S.S Butterfly pen.
            </p>
        </div>

    </div>

</section>


<!-- BUY MODAL -->
<div class="modal" id="buyModal">

    <div class="modal-box">

        <h2>🦋 S.S Butterfly Blue Pen</h2>

        <p>
            Thank you for choosing S.S Butterfly.
            Add your ordering details or connect this button
            to your preferred shopping/payment system.
        </p>

        <button class="close" onclick="closeModal()">
            Continue
        </button>

    </div>

</div>


<script>

/* Open Buy Modal */
function openModal(){
    document.getElementById("buyModal").style.display="flex";
}

/* Close Modal */
function closeModal(){
    document.getElementById("buyModal").style.display="none";
}

/* Scroll to product details */
function showDetails(){

    document.getElementById("details").scrollIntoView({
        behavior:"smooth"
    });

}


/* Close modal when clicking outside */
document.getElementById("buyModal").addEventListener("click",function(e){

    if(e.target === this){
        closeModal();
    }

});


/* Interactive 3D mouse movement */
const stage = document.getElementById("productStage");
const pen = document.getElementById("pen");

stage.addEventListener("mousemove",(e)=>{

    const rect = stage.getBoundingClientRect();

    const x = e.clientX - rect.left;
    const y = e.clientY - rect.top;

    const rotateY = (x / rect.width - .5) * 25;
    const rotateX = (y / rect.height - .5) * -18;

    pen.style.animation="none";

    pen.style.transform =
        `rotate(-20deg) rotateY(${rotateY}deg) rotateX(${rotateX}deg) translateY(-8px)`;

});

stage.addEventListener("mouseleave",()=>{

    pen.style.animation="penFloat 5s ease-in-out infinite";

});


/* Button click animation */
document.querySelectorAll(".btn").forEach(button=>{

    button.addEventListener("click",function(){

        this.style.transform="scale(.94)";

        setTimeout(()=>{
            this.style.transform="";
        },150);

    });

});


/* Small dynamic shine effect */
const barrel = document.querySelector(".barrel");

setInterval(()=>{

    barrel.style.filter="brightness(1.3)";

    setTimeout(()=>{
        barrel.style.filter="brightness(1)";
    },250);

},5000);

</script>

</body>
</html>
