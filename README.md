# valentine<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<title>💘 Question très sérieuse 💘</title>
<style>
body {
    margin: 0;
    height: 100vh;
    background: linear-gradient(135deg, #ff758c, #ff7eb3);
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: 'Comic Sans MS', cursive;
}

.card {
    background: white;
    padding: 30px;
    border-radius: 30px;
    text-align: center;
    width: 350px;
    box-shadow: 0 15px 40px rgba(0,0,0,0.3);
}

h1 {
    color: #ff3366;
}

.stickers {
    font-size: 42px;
    margin: 15px 0;
}

button {
    padding: 12px 25px;
    font-size: 18px;
    border-radius: 25px;
    border: none;
    cursor: pointer;
    margin: 10px;
}

#yes {
    background: #ff3366;
    color: white;
}

#no {
    background: #ccc;
    position: absolute;
}
</style>
</head>

<body>

<div class="card">
    <h1>Question ultra importante 💘</h1>

    <div class="stickers">
        🥰🌹💖🐻💌
    </div>

    <p>Est-ce que tu veux être<br><strong>ma Valentine ?</strong> 😍</p>

    <button id="yes" onclick="sayYes()">OUI 💖</button>
    <button id="no">NON 🙈</button>
</div>

<script>
const noBtn = document.getElementById("no");

noBtn.addEventListener("mouseover", () => {
    const x = Math.random() * (window.innerWidth - 100);
    const y = Math.random() * (window.innerHeight - 50);
    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
});

function sayYes() {
    window.location.href =
    "https://wa.me/?text=💘%20J’ai%20dit%20OUIII%20😍🌹%20Je%20suis%20ta%20Valentine%20💖";
}
</script>

</body>
</html>
