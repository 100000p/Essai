<!DOCTYPE html>
<html lang="en">
<head>
  <title>wilow</title>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    /* Style de base */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background:gray;
    }

    /* Style de la barre de navigation */
    .navbar {
      background-color: #333;
      overflow: hidden;
    }

    /* Style des liens de la barre de navigation */
    .navbar a {
      float: left;
      display: block;
      color: #f2f2f2;
      text-align: center;
      padding: 14px 16px;
      text-decoration: none;
    }

    /* Changement de style au survol */
    .navbar a:hover {
      background-color: #ddd;
      color: black;
    }

    /* Style du bouton de la version mobile */
    .navbar .icon {
      display: none;
    }

    /* Style pour les écrans plus petits (version mobile) */
    @media screen and (max-width: 600px) {
      .navbar a:not(:first-child) {display: none;}
      .navbar a.icon {
        float: right;
        display: block;
      }
    }

    /* Style pour la version mobile lorsque la barre de navigation est activée */
    @media screen and (max-width: 600px) {
      .navbar.responsive {
        position: relative;
      }
      .navbar.responsive a.icon {
        position: absolute;
        right: 0;
        top: 0;
      }
      .navbar.responsive a {
        float: none;
        display: block;
        text-align: left;
      }
    }
    input {
        margin:20px;
    }
    label {
        font-size:25px;
        color:silver;
        padding:10px;
    }
    body {
      
    }
    h1 {
     color:indigo;
     font-style:italic;
    
    }
    p {
     color:#ddd;
    
    }
    button{
    background:green;
   } 
   select {
    background:indigo;
    
    }
    
  </style>
</head>
<body>

<!--2 Barre de navigation -->
<div class="navbar" id="myNavbar">
<label>Menu</label>
  <a href="#Accueil">Accueil</a>
  <a href="#about">À propos</a>
  <a href="#" >Blog</a>
  <a href="javascript:void(0);" class="icon" onclick="myFunction()">
    <!-- Icône pour la version mobile -->
    &#9776;
  </a>
  </div>
<h1 id="animate" >Bienvenu dans ma page html</h1>
<p>Salut tout le monde ❗ </p>
<p>mes contacts sont disponibles dans le menu</p>
<button onclick="change();">contact</button>
<p id="para" ></p>
<h1 id="pa"></h1>
<p id="pata"></p>
 </video>
<!-- Script pour activer/désactiver la version mobile de la barre de navigation -->
<script>
function myFunction() {
  var x = document.getElementById("myNavbar");
  if (x.className === "navbar") {
    x.className += " responsive";
  } else {
    x.className = "navbar";
  }
}
const colors = ["#ff0000", "#00ff00", "#0000ff", "#ff00ff", "#ffff00"]; // Liste des couleurs à utiliser
let index = 0; // Index de la couleur actuelle

function changeColor() {
  const text = document.getElementById('animate');
  text.style.color = colors[index]; // Changer la couleur du texte
  index = (index + 1) % colors.length; // Passer à la prochaine couleur
}

setInterval(changeColor, 1000); // Appeler la fonction changeColor toutes les secondes
function change(){
var change= document.getElementById("para");
change.innerHTML="" ;

}
</script>
</body>
</html>

 
