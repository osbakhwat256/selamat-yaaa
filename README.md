# selamat-yaaa
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy Birthday 🐷🎀</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="card">
    <div class="sparkles">✨</div>
    <img src="https://cdn-icons-png.flaticon.com/512/616/616408.png" alt="Pig" class="pig-img">
    <h1>Happy Birthday, [Nama Temanmu] 🎉</h1>
    <p class="message">
      Semoga hari kamu seindah warna pink 🩷 dan seimut babi kecil ini 🐽  
      Terus bahagia, terus bersinar yaa 💫
    </p>
    <button onclick="toggleMusic()">💖 Play Music 💖</button>
    <audio id="music" src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_6fa1d1b1b9.mp3?filename=happy-birthday-117996.mp3"></audio>
  </div>

  <footer>Made with 🩷 by [Namamu]</footer>

  <script>
    function toggleMusic() {
      const music = document.getElementById('music');
      if (music.paused) {
        music.play();
      } else {
        music.pause();
      }
    }
  </script>
</body>
</html>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap');

body {
  background: linear-gradient(135deg, #ffd6e8, #ffe4f3);
  font-family: 'Poppins', sans-serif;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  margin: 0;
  overflow: hidden;
}

.card {
  background-color: #fff0f6;
  border-radius: 25px;
  padding: 40px;
  text-align: center;
  box-shadow: 0 10px 25px rgba(255, 155, 185, 0.4);
  max-width: 400px;
  animation: float 4s ease-in-out infinite;
  position: relative;
}

h1 {
  color: #ff82a9;
  margin-bottom: 15px;
}

.message {
  color: #d94f8a;
  font-size: 1rem;
  line-height: 1.5;
}

.pig-img {
  width: 100px;
  margin-bottom: 20px;
  animation: wiggle 3s infinite ease-in-out;
}

button {
  background-color: #ffb6c1;
  border: none;
  border-radius: 20px;
  padding: 10px 20px;
  color: white;
  font-size: 1rem;
  cursor: pointer;
  transition: 0.3s;
}

button:hover {
  background-color: #ff82a9;
}

footer {
  position: absolute;
  bottom: 20px;
  font-size: 0.8rem;
  color: #ff82a9;
}

@keyframes float {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-10px); }
}

@keyframes wiggle {
  0%, 100% { transform: rotate(0deg); }
  50% { transform: rotate(5deg); }
}

.sparkles {
  position: absolute;
  top: -15px;
  right: 20px;
  font-size: 1.5rem;
  animation: sparkle 2s infinite;
}

@keyframes sparkle {
  0%, 100% { opacity: 0.5; transform: scale(1); }
  50% { opacity: 1; transform: scale(1.3); }
}
