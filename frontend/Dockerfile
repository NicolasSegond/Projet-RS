# Utiliser l'image officielle Node.js
FROM node:14

# Définir le répertoire de travail
WORKDIR /app

# Copier les fichiers package.json et package-lock.json (s'il existe)
COPY package*.json ./

# Installer les dépendances
RUN npm install

# Copier tout le reste du projet dans le conteneur
COPY . .

# Exposer le port sur lequel l'application sera accessible
EXPOSE 8080

# Commande par défaut pour lancer l'application
CMD ["npm", "run", "serve"]
