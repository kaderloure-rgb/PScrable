<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>PScrable - Crypto Game</title>
<style>
  body { font-family: Arial, sans-serif; margin: 20px; background: #f4f4f9; color: #333; }
  h1 { text-align: center; color: #5a2a83; }
  #board { display: flex; flex-wrap: wrap; max-width: 300px; margin: 20px auto; }
  .tile { width: 60px; height: 60px; border: 1px solid #aaa; display: flex; justify-content: center; align-items: center; font-size: 18px; margin: 2px; background: #fff; cursor: pointer; }
  #wordInput { width: 80%; padding: 10px; font-size: 16px; margin: 10px auto; display: block; }
  #submitBtn { padding: 10px 20px; font-size: 16px; background: #5a2a83; color: #fff; border: none; cursor: pointer; }
  #message { text-align: center; font-weight: bold; margin-top: 15px; }
  #score { text-align: center; margin-top: 10px; font-size: 18px; }
</style>
</head>
<body>

<h1>PScrable - Crypto Game</h1>

<div id="board">
  <div class="tile">B</div>
  <div class="tile">L</div>
  <div class="tile">O</div>
  <div class="tile">C</div>
  <div class="tile">K</div>
  <div class="tile">C</div>
  <div class="tile">H</div>
  <div class="tile">A</div>
  <div class="tile">I</div>
  <div class="tile">N</div>
</div>

<input type="text" id="wordInput" placeholder="Entrez un mot crypto">
<button id="submitBtn">Valider</button>

<div id="message"></div>
<div id="score">Score : 0</div>

<script>
const validWords = ["BLOCK", "CHAIN", "TOKEN", "MINER", "NODE", "WALLET", "SMART", "CONTRACT", "LEDGER", "CRYPTO"];
let score = 0;

document.getElementById("submitBtn").addEventListener("click", function() {
  const input = document.getElementById("wordInput").value.toUpperCase().trim();
  const messageEl = document.getElementById("message");
  
  if(validWords.includes(input)) {
    score += input.length; 
    messageEl.textContent = "Bravo ! Mot correct : " + input;
  } else {
    messageEl.textContent = "Mot incorrect, essayez encore.";
  }
  
  document.getElementById("score").textContent = "Score : " + score;
  document.getElementById("wordInput").value = "";
});
</script>

</body>
</html><!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>PScrable</title>
</head>
<body>
  <h1>Bienvenue sur PScrable</h1>
  <p>Jeu de mots crypto en style Scrabble</p>
</body>
</html>PScrable
**Jeu de mots crypto style Scrabble**  
Formez des mots issus du vocabulaire blockchain pour gagner des fragments de Pi.  
Accessible via Pi Browser, avec plusieurs niveaux et un mode premium.
🔍 Fonctionnalités
- 🧠 Mots à deviner liés à la crypto et à la blockchain  
- 🎮 Niveaux progressifs et défis quotidiens  
- 💎 Mode premium avec récompenses en Pi  
- 🔐 Intégration du SDK Pi pour les paiements  
- 📱 Interface responsive et intuitive
🚀 Déploiement
L'application est hébergée sur Vercel :  
👉 [https://pscrable.vercel.app](https://pscrable.vercel.app)
🛠 Technologies
- HTML / CSS / JavaScript  
- SDK Pi Network  
- GitHub + Vercel
 👤 Auteur
Kader Loure — Éducateur visionnaire et créateur d'apps symboliques  
Passionné par l’innovation pédagogique, la narration et les technologies décentralisées.
 📬 Contact
Pour toute suggestion ou collaboration :  
📧 kaderloure@example.com *(à remplacer par ton vrai mail si tu veux)*  
🌐 [github.com/kader1](https://github.com/kader1)
