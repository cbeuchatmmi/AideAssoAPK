<template>
  <div class="min-h-screen flex flex-col bg-blue-100">
    <div class="flex-grow flex flex-col items-center justify-center">
      <h1 class="title flex items-center gap-2 text-blue-900">
        Téléchargez <img src="/src/assets/Logo_aide_asso.png" alt="Logo" class="h-8 w-auto" />
      </h1>
      <a href="/public/app-release.apk" download class="download-button">Télécharger l'APK</a>
    </div>
  </div>
</template>

<style scoped>
body {
  font-family: Arial, sans-serif;
  background-color: #f0f9ff; /* Fond blanc-bleu clair */
  color: #1e3a8a; /* Texte bleu foncé */
}

.title {
  font-size: 2rem;
  font-weight: bold;
  display: flex;
  align-items: center; /* Aligne verticalement le texte et l'image */
  gap: 0.5rem; /* Espacement entre le texte et l'image */
  margin-bottom: 10rem;

}

.download-button {
  padding: 12px 24px;
  background-color: #3b82f6; /* Bleu principal */
  color: white;
  border-radius: 8px;
  text-decoration: none;
  font-weight: bold;
  transition: background-color 0.3s ease;
}

.download-button:hover {
  background-color: #2563eb; /* Bleu plus foncé au survol */
}

footer {
  font-size: 0.9rem;
  color: #3b82f6; /* Bleu clair pour le footer */
  margin-top: auto; /* Pousse le footer vers le bas */
  text-align: center; /* Centre le texte du footer */
}
</style>