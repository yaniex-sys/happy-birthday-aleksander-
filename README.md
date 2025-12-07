# happy-birthday-aleksander-
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Aleksander Birthday Surprise</title>
<style>
    body {
        margin: 0;
        background: linear-gradient(135deg, #ffb3d9, #cce6ff);
        height: 100vh;
        display: flex;
        align-items: center;
        justify-content: center;
        font-family: "Poppins", sans-serif;
        overflow: hidden;
    }
    #popup {
        background: white;
        padding: 30px 40px;
        border-radius: 20px;
        text-align: center;
        font-size: 22px;
        box-shadow: 0 0 25px rgba(255, 0, 128, 0.4);
        animation: pop 0.6s ease;
    }
    @keyframes pop {
        0% { transform: scale(0); }
        70% { transform: scale(1.1); }
        100% { transform: scale(1); }
    }
    .confetti {
        position: fixed;
        top: -10px;
        width: 10px;
        height: 10px;
        background: hsl(calc(360 * var(--i)), 80%, 60%);
        animation: fall 2s linear infinite;
        left: calc(100% * var(--i));
    }
    @keyframes fall {
        to {
            transform: translateY(110vh) rotate(720deg);
        }
    }
</style>
</head>
<body>
<div id="popup">
    🎂 <b>Srećan rođendan, Aleksander!</b> 🎉<br>
    Želim ti puno sreće, ljubavi i lepih trenutaka! ✨💖
</div>
<script>
function birthdayGreeting() {
    alert("🎂 Srećan rođendan, Aleksander! 🎉\\nŽelim ti puno sreće, ljubavi i lepih trenutaka! ✨");
}
birthdayGreeting();
for (let i = 0; i < 50; i++) {
    let c = document.createElement("div");
    c.classList.add("confetti");
    c.style.setProperty("--i", Math.random());
    document.body.appendChild(c);
}
</script>
</body>
</html>
