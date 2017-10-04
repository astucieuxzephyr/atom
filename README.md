# Editeur ATOM - Sauvegarde des paramètres sur GitHub
-----------------------------------------------------

**Rappels :**
- Sous Windows, ces fichiers doivent se trouver dans le dossier C:\Users\NomUtilisateur\.atom
- Site Editeur Atom : https://atom.io/

## Pour récupérer ce projet sur votre PC (sous Windows) :
* Ci-dessous, changer le NomUtilisateur avec celui de votre PC
    > cd C:\Users\NomUtilisateur\.atom
    > git clone https://github.com/astucieuxzephyr/atom
* Récupérer les packages automatiquement sur votre PC
    > apm install --packages-file package.list
    - Ou bien (si vous êtes dans un autre dossier)
        > apm install --packages-file ~/.atom/package.list

## Pour maintenir ce projet à jour sur GitHub :

* Sous Windows, se placer dans le dossier de config d'atom
    > cd C:\Users\NomUtilisateur\.atom
* Télécharger d'éventuels changements
    > git pull atom master
* Mettre à jour le fichier de qui contient la liste des packages
    > apm list --installed --bare > package.list
    - Ou bien (si vous êtes dans un autre dossier)
        > apm list --installed --bare > ~/.atom/package.list
* Mettre les fichiers modifiés dans le stage :
    > git add \*.\*
* Commit des fichiers en local
    > git commit -m "Mise à jour des fichiers de config Atom"
* Mise à jour du repo sur GitHub
    > git push atom master
