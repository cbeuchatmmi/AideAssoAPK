<template>
  <div class="container">
    <div class="content">
      <h1 class="title">
        Téléchargez <img src="/src/assets/Logo_aide_asso.png" alt="Logo" class="logo" />
      </h1>
      <a href="/app-release.apk" download class="download-button">
        Télécharger l'APK
      </a>
    </div>
    <footer class="footer">
      © 2025 Mon Application
    </footer>
  </div>
</template>

<style scoped>


/* Contenu principal */
.content {
  flex-grow: 1; /* Permet au contenu de s'étendre pour occuper l'espace disponible */
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 16px; /* Ajoute un padding pour éviter que le contenu touche les bords */
}

/* Titre */
.title {
  font-size: 2rem; /* Taille du titre pour les grands écrans */
  font-weight: bold;
  display: flex;
  align-items: center; /* Aligne verticalement le texte et l'image */
  gap: 16px; /* Espacement entre le texte et l'image */
  text-align: center;
  margin-bottom: 24px;
}

/* Logo */
.logo {
  height: 3rem; /* Taille du logo pour les grands écrans */
  width: auto;
}

/* Bouton de téléchargement */
.download-button {
  padding: 16px 32px; /* Taille du bouton pour les grands écrans */
  background-color: #3b82f6; /* Bleu principal */
  color: white;
  border-radius: 8px;
  text-decoration: none;
  font-weight: bold;
  text-align: center;
  transition: background-color 0.3s ease;
  display: inline-block;
  font-size: 1rem; /* Taille du texte du bouton */
}

.download-button:hover {
  background-color: #2563eb; /* Bleu plus foncé au survol */
}

/* Footer */
.footer {
  font-size: 1rem; /* Taille du texte du footer pour les grands écrans */
  color: #3b82f6; /* Bleu clair pour le footer */
  margin-top: auto; /* Pousse le footer vers le bas */
  text-align: center;
  padding: 16px;
}

/* Media queries pour les petits écrans */
@media (max-width: 640px) {
  .title {
    font-size: 1.25rem; /* Réduit la taille du titre sur mobile */
    flex-direction: column; /* Place le texte et l'image en colonne */
    gap: 8px; /* Réduit l'espacement entre le texte et l'image */
  }

  .logo {
    height: 1.5rem; /* Réduit la taille du logo sur mobile */
  }

  .download-button {
    width: 100%; /* Le bouton occupe toute la largeur sur mobile */
    padding: 12px; /* Ajuste le padding pour les petits écrans */
    font-size: 0.9rem; /* Réduit la taille du texte du bouton */
  }

  .footer {
    font-size: 0.8rem; /* Réduit la taille du texte du footer sur mobile */
  }
}

/* Media queries pour les grands écrans */
@media (min-width: 1024px) {
  .content {
    max-width: 800px; /* Limite la largeur du contenu sur les grands écrans */
    margin: 0 auto; /* Centre le contenu horizontalement */
  }

  .title {
    font-size: 2.5rem; /* Augmente la taille du titre sur les grands écrans */
  }

  .logo {
    height: 4rem; /* Augmente la taille du logo sur les grands écrans */
  }

  .download-button {
    font-size: 1.25rem; /* Augmente la taille du texte du bouton */
    padding: 20px 40px; /* Augmente la taille du bouton */
  }

  .footer {
    font-size: 1.1rem; /* Augmente la taille du texte du footer */
  }
}
</style>