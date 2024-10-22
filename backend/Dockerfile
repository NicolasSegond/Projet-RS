# Utilise l'image officielle Node.js
FROM node:14

# Définir le répertoire de travail
WORKDIR /app

# Copier les fichiers package.json et installer les dépendances
COPY package.json ./
RUN npm install

# Copier tout le reste du projet
COPY . .

# Exposer le port sur lequel le backend sera accessible
EXPOSE 3000

# Commande par défaut pour lancer le serveur
CMD ["npm", "start"]
