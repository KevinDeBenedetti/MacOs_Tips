# Installer Homebrew ~ Php ~ MySQL ~ Apache HTTP sur MacOS
![macOS Badge](https://img.shields.io/badge/macOS-000?logo=macos&logoColor=fff&style=flat-square)![Homebrew Badge](https://img.shields.io/badge/Homebrew-FBB040?logo=homebrew&logoColor=fff&style=flat-square)![PHP Badge](https://img.shields.io/badge/PHP-777BB4?logo=php&logoColor=fff&style=flat-square)![MySQL Badge](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=fff&style=flat-square)![Apache Badge](https://img.shields.io/badge/Apache-D22128?logo=apache&logoColor=fff&style=flat-square) <br>
Installation de Php ~ MySQL ~ Apache HTTP Serveur sur macOS
## SOMMAIRE
* [Installer homebrew](#Installer-homebrew)
* [Installer PHP](#Installer-PHP)
* [Installer MySQL](#Installer-MySQL)
* [Installer Apache HTTP Serveur](#Installer-Apache-HTTP-Serveur)


<br>
<br>

![Homebrew Badge](https://img.shields.io/badge/Homebrew-FBB040?logo=homebrew&logoColor=fff&style=plastic)
<hr>

##  Installer homebrew
Le site officiel ➡️ [https://brew.sh/index_fr](https://brew.sh/index_fr) <br>

#### 💻 Les commandes pour l'installation

```
// Installation de hombrew
mclovin@mac ~ % /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

mclovin@mac ~ % brew install wget
```

#### 💻  Les commandes de bases
```
mclovin@mac ~ % brew update
mclovin@mac ~ % brew upgrade
mclovin@mac ~ % brew install
mclovin@mac ~ % brew uninstall
mclovin@mac ~ % brew info
mclovin@mac ~ % brew list
mclovin@mac ~ % brew search
```

### Documentation <br>
📒 [https://docs.brew.sh](https://docs.brew.sh)

<br>
<br>

![PHP Badge](https://img.shields.io/badge/PHP-777BB4?logo=php&logoColor=fff&style=flat)
<hr>

##  Installer PHP

#### 💻 Commande pour chercher les versions de php disponibles à l'installation 

```
mclovin@mac ~ % brew search php
==> Formulae
brew-php-switcher        php-cs-fixer@2           phpbrew                  phpstan
php                      php@7.4                  phplint                  phpunit
php-code-sniffer         php@8.0                  phpmd                    pcp
php-cs-fixer             php@8.1                  phpmyadmin               pup
```
#### 💻 Commande pour installer la version choisie (php@8.1 pour l'exemple)
```
mclovin@mac ~ % brew install php@8.1
```
#### 💡 Info - Commandes pour accéder au répertoire d'installation
```
mclovin@mac ~ % cd /usr/local/etc
mclovin@mac ~ % ls /usr/local/etc
```
### Documentation <br>
📒 [https://formulae.brew.sh/formula/php#default](https://formulae.brew.sh/formula/php#default)

<br>
<br>


![MySQL Badge](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=fff&style=flat)
<hr>

## Installer MySQL 

#### 💻 Commande pour installer MySQL
```
mclovin@mac ~ % brew install mysql
```
#### Les commandes de base

⬇️ Se connectter avec l'utilisateur root
```
mclovin@mac ~ % mysql -u root -p
```
⬇️ Charger une bdd à partir d'un fichier
```
mclovin@mac ~ % mysql -u root -p nom_de_la_base_de_donnees < nom_du_fichier.sql
```
### Documentation <br>
📒 [https://formulae.brew.sh/formula/mysql#default](https://formulae.brew.sh/formula/mysql#default)

<br>
<br>

![Apache Badge](https://img.shields.io/badge/Apache-D22128?logo=apache&logoColor=fff&style=flat)
<hr>

## Installer Apache HTTP Serveur

#### 💻 Commande pour installer httpd
```
mclovin@mac ~ % brew install httpd
```
#### 💻 Commande pour ouvrir httpd au démarrage
```
mclovin@mac ~ % sudo brew services start httpd
```
#### 💡 Info - URL : http://localhost:8080
#### 💻 Configurer httpd
```
mclovin@mac ~ % nano /usr/local/etc/httpd/httpd.conf
```
#### 💻 Définir le port Apache dans httpd.conf
```
Listen 8080
// A modifier
Listen 80
```
#### 💻 Créer un document racine
Par défaut : /usr/local/var/www
```
mclovin@mac ~ % mkdir Sites
```
#### 💻 Modifier la racine du document dans httpd.conf
Par défaut : /usr/local/var/www
```
DocumentRoot /Users/mclovin/Sites
```
#### Les commandes de base

⬇️ Lancer Apache
```
mclovin@mac ~ % sudo /usr/local/opt/apache2/bin/apachectl start
```
⬇️ Arrêter Apache
```
mclovin@mac ~ % sudo /usr/local/opt/apache2/bin/apachectl stop

```
⬇️ Lancer Apache
```
mclovin@mac ~ % sudo apachestl start 

```
⬇️ Arrêter Apache
```
mclovin@mac ~ % sudo apachestl stop 

```
⬇️ Redémarrer Apache
```
mclovin@mac ~ % sudo apachestl restart 

```

### La documentation <br>
📒 [https://formulae.brew.sh/formula/httpd#default](https://formulae.brew.sh/formula/httpd#default)

📒 [https://httpd.apache.org](https://httpd.apache.org)

### Sources
📚 [https://tecadmin.net/install-apache-macos-homebrew/](https://tecadmin.net/install-apache-macos-homebrew/)

📚 [https://www.php.net/manual/fr/install.unix.apache2.php](https://www.php.net/manual/fr/install.unix.apache2.php)