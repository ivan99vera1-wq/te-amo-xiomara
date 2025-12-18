<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Te amo Xiomara</title>

<style>
body {
    margin: 0;
    min-height: 100vh;
    background: linear-gradient(135deg, #ff5f6d, #ffc371);
    overflow: hidden;
    font-family: Arial, sans-serif;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
}

.contenedor {
    background: rgba(0,0,0,0.35);
    padding: 25px;
    border-radius: 25px;
    text-align: center;
    max-width: 360px;
    z-index: 2;
}

img {
    width: 100%;
    border-radius: 20px;
    margin-bottom: 15px;
}

h1 {
    font-size: 2.4em;
}

p {
    font-size: 1.2em;
}

.heart {
    position: absolute;
    bottom: -20px;
    font-size: 20px;
    animation: subir 6s linear infinite;
}

@keyframes subir {
    0% { transform: translateY(0); opacity: 1; }
    100% { transform: translateY(-120vh); opacity: 0; }
}
</style>
</head>

<body>

<div class="contenedor">
    <img src="foto.jpg">
    <h1>❤️ Te amo Xiomara ❤️</h1>
    <p>
        Este lugar existe solo para decirte  
        lo importante que eres para mí  
        y lo mucho que te amo.
    </p>
</div>

<script>
setInterval(() => {
    const c = document.createElement("div");
    c.className = "heart";
    c.innerText = "❤️";
    c.style.left = Math.random() * 100 + "vw";
    c.style.fontSize = (Math.random() * 20 + 15) + "px";
    document.body.appendChild(c);
    setTimeout(() => c.remove(), 6000);
}, 300);
</script>

</body>
</html>
