<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Chúc Mừng Ngày 20/10 💖</title>
<style>
  html, body {
    margin: 0;
    padding: 0;
    overflow: hidden;
    height: 100%;
    background: linear-gradient(180deg, #ffd6e8 0%, #ffb6c1 50%, #ffeaf0 100%);
    font-family: "Segoe UI", sans-serif;
  }

  h1 {
    position: absolute;
    top: 40%;
    width: 100%;
    text-align: center;
    color: white;
    font-size: 40px;
    text-shadow: 0 0 15px rgba(255, 255, 255, 0.9);
    opacity: 0;
    animation: fadeIn 5s ease-in-out forwards;
  }

  @keyframes fadeIn {
    0% { opacity: 0; transform: translateY(20px); }
    100% { opacity: 1; transform: translateY(0); }
  }

  .heart {
    position: absolute;
    width: 20px;
    height: 20px;
    background-color: rgba(255, 105, 180, 0.9);
    transform: rotate(45deg);
    animation: float 6s linear infinite;
  }

  .heart::before,
  .heart::after {
    content: '';
    position: absolute;
    width: 20px;
    height: 20px;
    background-color: rgba(255, 105, 180, 0.9);
    border-radius: 50%;
  }

  .heart::before {
    top: -10px;
    left: 0;
  }

  .heart::after {
    top: 0;
    left: -10px;
  }

  @keyframes float {
    0% {
      transform: translateY(0) rotate(45deg) scale(1);
      opacity: 1;
    }
    100% {
      transform: translateY(-800px) rotate(45deg) scale(1.3);
      opacity: 0;
    }
  }

  footer {
    position: absolute;
    bottom: 20px;
    width: 100%;
    text-align: center;
    font-size: 18px;
    color: #fff;
    opacity: 0.8;
    font-style: italic;
  }
</style>
</head>
<body>
<h1>💖 Chúc Mừng Ngày 20/10 💖</h1>
<footer>Gửi đến em — người khiến thế giới này dịu dàng hơn 🌸</footer>

<script>
function createHeart() {
  const heart = document.createElement('div');
  heart.classList.add('heart');
  document.body.appendChild(heart);

  const size = Math.random() * 15 + 10;
  heart.style.width = size + 'px';
  heart.style.height = size + 'px';
  heart.style.left = Math.random() * window.innerWidth + 'px';
  heart.style.backgroundColor = `rgba(255, ${100 + Math.random()*80}, ${150 + Math.random()*100}, 0.9)`;
  heart.style.animationDuration = 5 + Math.random() * 3 + 's';

  setTimeout(() => {
    heart.remove();
  }, 8000);
}

setInterval(createHeart, 200);
</script>
</body>
</html>
