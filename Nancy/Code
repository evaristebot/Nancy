<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Pour Nancy ❤️</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Arial', sans-serif;
      overflow-x: hidden;
      background: linear-gradient(135deg, #fff5f5 0%, #ffecec 100%);
    }
    
    /* Bouton super stylé */
    #surpriseBtn {
      position: fixed;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      padding: 20px 40px;
      background: linear-gradient(45deg, #ff6b9d, #ff8e53);
      color: white;
      border: none;
      border-radius: 50px;
      font-size: 24px;
      font-weight: bold;
      cursor: pointer;
      box-shadow: 0 10px 20px rgba(255, 105, 157, 0.3),
                  0 6px 6px rgba(255, 105, 157, 0.2),
                  inset 0 -2px 5px rgba(0,0,0,0.1),
                  inset 0 2px 5px rgba(255,255,255,0.5);
      transition: all 0.4s ease;
      z-index: 100;
      text-transform: uppercase;
      letter-spacing: 2px;
      overflow: hidden;
    }
    
    #surpriseBtn:hover {
      transform: translate(-50%, -50%) scale(1.05);
      box-shadow: 0 15px 30px rgba(255, 105, 157, 0.4),
                  0 10px 10px rgba(255, 105, 157, 0.3),
                  inset 0 -2px 5px rgba(0,0,0,0.1),
                  inset 0 2px 5px rgba(255,255,255,0.5);
      animation: pulse 1.5s infinite;
    }
    
    #surpriseBtn:active {
      transform: translate(-50%, -50%) scale(0.95);
    }
    
    #surpriseBtn::after {
      content: '';
      position: absolute;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: linear-gradient(
        to bottom right,
        rgba(255,255,255,0) 0%,
        rgba(255,255,255,0) 45%,
        rgba(255,255,255,0.5) 48%,
        rgba(255,255,255,0) 52%,
        rgba(255,255,255,0) 100%
      );
      transform: rotate(30deg);
      transition: all 0.3s;
    }
    
    #surpriseBtn:hover::after {
      left: 100%;
      top: 100%;
    }
    
    /* Animation du texte "salut Nancy" */
    #salut {
      position: fixed;
      top: 40%;
      left: 50%;
      transform: translate(-50%, -50%);
      font-size: 3rem;
      color: #ff6b9d;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
      opacity: 1;
      transition: all 1s ease-out;
      z-index: 10;
      font-weight: bold;
      text-align: center;
    }
    
    #salut.fly-away {
      top: -100%;
      opacity: 0;
      transform: translate(-50%, -50%) rotate(10deg);
    }
    
    /* Message d'amour */
    #loveMessage {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      display: none;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      z-index: 5;
    }
    
    /* Effets de particules améliorés */
    .particles {
      position: absolute;
      width: 100%;
      height: 100%;
      overflow: hidden;
      z-index: 1;
    }
    
    .particle {
      position: absolute;
      background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path fill="%23ff6b9d" d="M12,21.35L10.55,20.03C5.4,15.36 2,12.27 2,8.5C2,5.41 4.42,3 7.5,3C9.24,3 10.91,3.81 12,5.08C13.09,3.81 14.76,3 16.5,3C19.58,3 22,5.41 22,8.5C22,12.27 18.6,15.36 13.45,20.03L12,21.35Z"/></svg>') no-repeat center center;
      background-size: contain;
      opacity: 0;
      animation: float-up 6s linear infinite;
    }
    
    /* Animations */
    @keyframes pulse {
      0% { transform: translate(-50%, -50%) scale(1); }
      50% { transform: translate(-50%, -50%) scale(1.1); }
      100% { transform: translate(-50%, -50%) scale(1); }
    }
    
    @keyframes float-up {
      0% {
        transform: translateY(100vh) rotate(0deg) scale(0.5);
        opacity: 0;
      }
      10% {
        opacity: 0.8;
      }
      90% {
        opacity: 0.8;
      }
      100% {
        transform: translateY(-100px) rotate(360deg) scale(1.2);
        opacity: 0;
      }
    }
    
    /* Message d'amour stylé */
    .love-content {
      text-align: center;
      z-index: 2;
      animation: fadeIn 2s ease-out;
    }
    
    .love-content h1 {
      font-size: 4rem;
      color: #ff6b9d;
      margin-bottom: 20px;
      text-shadow: 3px 3px 6px rgba(0, 0, 0, 0.1);
      background: linear-gradient(45deg, #ff6b9d, #ff8e53);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: textGlow 2s infinite alternate;
    }
    
    .love-content p {
      font-size: 1.8rem;
      color: #9c27b0;
      margin: 10px 0;
      opacity: 0;
      animation: fadeInUp 1s forwards;
    }
    
    .love-content p:nth-child(2) {
      animation-delay: 0.5s;
    }
    
    .love-content p:nth-child(3) {
      animation-delay: 1s;
    }
    
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    
    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    
    @keyframes textGlow {
      from { text-shadow: 0 0 10px rgba(255,107,157,0.3); }
      to { text-shadow: 0 0 20px rgba(255,107,157,0.6); }
    }
  </style>
</head>
<body>
  <button id="surpriseBtn">Clique ici, Nancy ❤️</button>
  
  <div id="salut">
    salut Nancy
  </div>

  <div id="loveMessage">
    <div class="particles" id="particles"></div>
    <div class="love-content">
      <h1>Je t'aime Nancy ❤️</h1>
      <p>♡ ∞ + ♡ = T○I ♡</p>
      <p>Tu illuminés mon univers ✨</p>
    </div>
  </div>

  <!-- Audio optionnel (décommenter pour activer) -->
  <!--
  <audio id="romanticMusic" loop>
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
  </audio>
  -->

  <script>
    // Création des particules
    function createParticles() {
      const container = document.getElementById('particles');
      const particleCount = 50;
      
      for (let i = 0; i < particleCount; i++) {
        const particle = document.createElement('div');
        particle.classList.add('particle');
        
        // Position aléatoire
        particle.style.left = Math.random() * 100 + 'vw';
        
        // Taille aléatoire
        const size = Math.random() * 20 + 10;
        particle.style.width = size + 'px';
        particle.style.height = size + 'px';
        
        // Animation avec délai aléatoire
        particle.style.animationDuration = (Math.random() * 3 + 3) + 's';
        particle.style.animationDelay = (Math.random() * 5) + 's';
        
        container.appendChild(particle);
      }
    }
    
    // Gestion du clic sur le bouton
    document.getElementById('surpriseBtn').addEventListener('click', function() {
      // Animation du bouton
      this.style.transform = 'translate(-50%, -50%) scale(1.2)';
      this.style.opacity = '0';
      
      // Animation du texte "salut Nancy"
      document.getElementById('salut').classList.add('fly-away');
      
      // Démarrer la musique (optionnel)
      // document.getElementById('romanticMusic').play();
      
      // Afficher le message d'amour après un délai
      setTimeout(function() {
        document.getElementById('loveMessage').style.display = 'flex';
        createParticles();
      }, 1000);
    });
  </script>
</body>
</html>
