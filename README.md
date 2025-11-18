Mon Projet Netmiko

Initialiser un dépôt Git local

mkdir meryem-elheni-netmiko
cd meryem-elheni-netmiko
git init

 Ajouter et commiter des fichiers

nano README.md
git add README.md
git commit -m "Ajout du fichier README"

nano main.py
git add main.py
git commit -m "Ajout du script Python principal"

git log --oneline --graph


git checkout -b feature/netmiko

git add main.py
git commit -m "Ajout de la fonction acces_netmiko"

git checkout master
git merge feature/netmiko


git remote add origin https://github.com/meryemelheni/meryem-elheni-netmiko.git
git push -u origin master

git fetch origin
git checkout -b feature/salut origin/feature/salut

git add main.py
git commit -m "Ajout de la fonction dire_salut"
git push origin feature/salut

git checkout master
git pull origin master

O

