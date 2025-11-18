# Mon Projet Netmiko

Ce projet utilise Netmiko pour se connecter à un routeur Cisco, afficher la date et récupérer les interfaces dans un fichier.

---

## I. Initialiser un dépôt Git local

mkdir meryem-elheni-netmiko
cd meryem-elheni-netmiko
git init

---

## II. Ajouter et commiter des fichiers

nano README.md
git add README.md
git commit -m "Ajout du fichier README"

nano main.py
git add main.py
git commit -m "Ajout du script Python principal"

git log --oneline --graph

---

## III. Créer et fusionner des branches

git checkout -b feature/netmiko

git add main.py
git commit -m "Ajout de la fonction acces_netmiko"

git checkout master
git merge feature/netmiko

---

## IV. Travailler avec GitHub

git remote add origin https://github.com/meryemelheni/meryem-elheni-netmiko.git
git push -u origin master

git fetch origin
git checkout -b feature/salut origin/feature/salut

git add main.py
git commit -m "Ajout de la fonction dire_salut"
git push origin feature/salut

git checkout master
git pull origin master

