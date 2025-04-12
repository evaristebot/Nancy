<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Joyeux Anniversaire Nancy</title>
  <style>
    body {
      background: linear-gradient(to bottom right, #ffdee9, #b5fffc);
      font-family: 'Arial', sans-serif;
      text-align: center;
      padding: 50px;
      animation: fadeIn 2s ease-in-out;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: scale(0.9); }
      to { opacity: 1; transform: scale(1); }
    }

    h1 {
      font-size: 3em;
      color: #ff4d88;
      margin-bottom: 10px;
      animation: bounce 1.5s infinite;
    }

    @keyframes bounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }

    .photo {
      border-radius: 20px;
      max-width: 300px;
      margin: 20px auto;
      box-shadow: 0 0 20px #ff99cc;
      border: 4px solid white;
    }

    .message {
      font-size: 1.5em;
      color: #333;
      margin-top: 20px;
      line-height: 1.6;
    }

    .coeur {
      font-size: 2.5em;
      color: red;
      margin-top: 30px;
      animation: pulse 1.5s infinite;
    }

    @keyframes pulse {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.2); }
    }
  </style>
</head>
<body>
  <h1>♡ Joyeux Anniversaire ♡</h1>
  <h2>Nancy</h2>
  <img class="photo" src="Messenger_creation_5861B096-E499-4655-BF9B-D9925E3B2738.jpeg" alt="Photo de Nancy">
  <div class="message">
    En ce jour spécial, je veux te souhaiter tout le bonheur que tu mérites.<br>
    Ton sourire illumine le monde et ton énergie rend chaque moment magique.<br>
    Que cette année t’apporte encore plus de rêves réalisés et d’étoiles dans les yeux.
  </div>
  <div class="coeur">Je t’aime Nancy</div>
</body>
</html> 
