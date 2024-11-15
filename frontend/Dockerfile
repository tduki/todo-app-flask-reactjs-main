# Étape 1 : Construire l'application React
FROM node:18 AS builder

WORKDIR /app

# Copier les fichiers nécessaires pour installer les dépendances
COPY package*.json ./

# Installer les dépendances
RUN npm install

# Copier tout le code source
COPY . .

# Construire le projet pour la production
RUN npm run build

# Étape 2 : Servir les fichiers statiques avec Nginx
FROM nginx:alpine

# Copier les fichiers construits dans le répertoire de Nginx
COPY --from=builder /app/dist /usr/share/nginx/html

# Exposer le port 80
EXPOSE 3000

# Commande pour démarrer Nginx
CMD ["nginx", "-g", "daemon off;"]
