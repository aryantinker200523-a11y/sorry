<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Sorry Jaic 💗</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: url('https://upload.wikimedia.org/wikipedia/commons/e/e6/Paris_-_Eiffel_Tower_view_from_Trocad%C3%A9ro_02.jpg') no-repeat center center fixed;
      background-size: cover;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      font-family: 'Comic Sans MS', cursive, sans-serif;
    }

    .container {
      text-align: center;
      position: relative;
    }

    .monkey {
      max-width: 300px;
      animation: float 3s ease-in-out infinite;
      z-index: 2;
      position: relative;
    }

    .speech-bubble {
      position: absolute;
      top: -80px;
      left: 50%;
      transform: translateX(-50%);
      background: rgba(255, 255, 255, 0.9);
      border-radius: 10px;
      padding: 10px 20px;
      border: 2px solid #ff69b4;
      font-size: 1.2rem;
      color: #ff1493;
      box-shadow: 2px 4px 8px rgba(0, 0, 0, 0.2);
      animation: popIn 1.5s ease forwards;
      z-index: 3;
    }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }

    @keyframes popIn {
      0% { opacity: 0; transform: scale(0.5); }
      100% { opacity: 1; transform: scale(1); }
    }

    @media (max-width: 500px) {
      .speech-bubble {
        font-size: 1rem;
        padding: 8px 16px;
        top: -70px;
      }
      .monkey {
        max-width: 200px;
      }
    }
  </style>
</head>
<body>

  <div class="container">
    <div class="speech-bubble">Sorry Jaic 💗</div>
    <img
      class="monkey"
      src="https://cdn.pixabay.com/photo/2017/08/30/21/42/monkey-2697337_1280.png"
      alt="Monkey holding ice cream"
    >
  </div>

</body>
</html>
