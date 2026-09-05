<!DOCTYPE html>
<html lang="hu">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080808">

<title>GTA VI</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html, body {
    width: 100%;
    height: 100%;
    overflow: hidden;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: #080808;
    color: white;
}

/* ===== GTA VI HÁTTÉR ===== */

.background {
    position: fixed;
    inset: 0;

    background:
        radial-gradient(
            ellipse at 25% 25%,
            rgba(255, 90, 160, .45),
            transparent 38%
        ),
        radial-gradient(
            ellipse at 75% 35%,
            rgba(255, 170, 80, .35),
            transparent 35%
        ),
        radial-gradient(
            ellipse at 50% 100%,
            rgba(40, 90, 170, .35),
            transparent 45%
        ),
        linear-gradient(
            145deg,
            #190b22,
            #4b173b 38%,
            #111d3c 72%,
            #050509
        );

    transform: scale(1.05);
    animation: backgroundMove 12s ease-in-out infinite alternate;
}

/* Napfényes GTA-hangulatú fényfoltok */
.background::before {
    content: "";
    position: absolute;
    inset: -20%;

    background:
        radial-gradient(
            circle at 35% 30%,
            rgba(255,255,255,.18),
            transparent 8%
        ),
        radial-gradient(
            circle at 70% 55%,
            rgba(255,100,160,.15),
            transparent 15%
        );

    filter: blur(25px);
}

/* Sötétítés */
.dark {
    position: fixed;
    inset: 0;

    background:
        linear-gradient(
            to bottom,
            rgba(0,0,0,.05),
            rgba(0,0,0,.55)
        );

    z-index: 1;
}

/* ===== BETÖLTŐ ===== */

#loadingScreen {
    position: fixed;
    inset: 0;

    z-index: 5;

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    text-align: center;

    transition:
        opacity 1.2s ease,
        transform 1.2s ease;
}

.logo {
    font-size: clamp(75px, 18vw, 190px);
    font-weight: 1000;

    letter-spacing: 10px;

    text-shadow:
        0 4px 20px rgba(0,0,0,.9),
        0 0 35px rgba(255,255,255,.25);

    animation:
        logoAppear 1.8s cubic-bezier(.2,.8,.2,1);
}

.subtitle {
    margin-top: -8px;

    font-size: clamp(10px, 2vw, 14px);
    letter-spacing: 8px;

    opacity: .8;

    text-shadow:
        0 2px 8px black;
}

/* ===== PROGRESS BAR ===== */

.loading {
    position: absolute;

    left: 50%;
    bottom: 9%;

    transform: translateX(-50%);

    width: min(560px, 78%);
}

.loadingInfo {
    display: flex;
    justify-content: space-between;

    margin-bottom: 9px;

    font-size: 11px;
    letter-spacing: 2px;

    opacity: .8;
}

.bar {
    width: 100%;
    height: 5px;

    border-radius: 20px;

    background: rgba(255,255,255,.25);

    overflow: hidden;

    box-shadow:
        0 2px 15px rgba(0,0,0,.7);
}

.progress {
    width: 0%;
    height: 100%;

    background: white;

    border-radius: 20px;

    box-shadow:
        0 0 12px white,
        0 0 25px rgba(255,255,255,.6);

    transition: width .15s linear;
}

/* ===== PRANK ===== */

#prankScreen {
    position: fixed;
    inset: 0;

    z-index: 20;

    display: none;

    justify-content: center;
    align-items: center;

    flex-direction: column;

    text-align: center;

    background:
        radial-gradient(
            circle,
            #260006 0%,
            #090000 48%,
            #000 100%
        );

    animation: prankIn .8s ease;
}

.prankTitle {
    font-size: clamp(65px, 17vw, 190px);

    font-weight: 1000;

    letter-spacing: 7px;

    color: #ff1744;

    text-shadow:
        0 0 10px #ff1744,
        0 0 30px rgba(255,23,68,.9),
        0 0 75px rgba(255,23,68,.55);

    animation:
        glitch .12s infinite alternate;
}

.prankText {
    margin-top: 15px;

    font-size: clamp(12px, 3vw, 20px);

    letter-spacing: 4px;

    opacity: .8;
}

/* ===== ANIMÁCIÓK ===== */

@keyframes logoAppear {
    0% {
        opacity: 0;
        transform: scale(.65);
        filter: blur(20px);
    }

    100% {
        opacity: 1;
        transform: scale(1);
        filter: blur(0);
    }
}

@keyframes backgroundMove {
    0% {
        transform: scale(1.05) translate(-1%, -1%);
    }

    100% {
        transform: scale(1.12) translate(1%, 1%);
    }
}

@keyframes prankIn {
    from {
        opacity: 0;
        transform: scale(1.08);
    }

    to {
        opacity: 1;
        transform: scale(1);
    }
}

@keyframes glitch {
    from {
        transform: translateX(-2px);
    }

    to {
        transform: translateX(2px);
    }
}
</style>
</head>

<body>

<!-- Háttér -->
<div class="background"></div>
<div class="dark"></div>

<!-- GTA VI betöltőképernyő -->
<div id="loadingScreen">

    <div class="logo">
        GTA VI
    </div>

    <div class="subtitle">
        LOADING EXPERIENCE
    </div>

    <div class="loading">

        <div class="loadingInfo">
            <span>INITIALIZING...</span>
            <span id="percent">0%</span>
        </div>

        <div class="bar">
            <div
                class="progress"
                id="progress">
            </div>
        </div>

    </div>

</div>

<!-- Prank képernyő -->
<div id="prankScreen">

    <div class="prankTitle">
        PRANK 😂
    </div>

    <div class="prankText">
        NYUGI, EZ CSAK EGY PRANK VOLT 😭
    </div>

</div>

<script>

let progress = 0;

const progressBar =
    document.getElementById("progress");

const percent =
    document.getElementById("percent");

const loadingScreen =
    document.getElementById("loadingScreen");

const prankScreen =
    document.getElementById("prankScreen");


/* Betöltés */
const loader = setInterval(() => {

    /* Véletlenszerűen halad */
    progress +=
        Math.floor(Math.random() * 3) + 1;

    if (progress >= 100) {

        progress = 100;

        clearInterval(loader);

        /* Kis várakozás 100% után */
        setTimeout(() => {

            loadingScreen.style.opacity = "0";
            loadingScreen.style.transform =
                "scale(1.04)";

            setTimeout(() => {

                loadingScreen.style.display =
                    "none";

                prankScreen.style.display =
                    "flex";

            }, 1200);

        }, 900);
    }

    progressBar.style.width =
        progress + "%";

    percent.textContent =
        progress + "%";

}, 120);

</script>

</body>
</html>
