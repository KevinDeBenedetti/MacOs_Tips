# Install-Php_MySQL_ApacheHTTP-MacOS
Installation de Php ~ MySQL ~ Apache HTTP Serveur sur macOS

## SOMMAIRE
* [Installer homebrew](#Installer-homebrew)
* [Installer PHP](#Installer-PHP)
* [Installer MySQL](#Installer-MySQL)

<br>

## ![Homebrew Badge](https://img.shields.io/badge/Homebrew-FBB040?logo=homebrew&logoColor=fff&style=plastic) Installer homebrew
Le site officiel ➡️ [https://brew.sh/index_fr](https://brew.sh/index_fr) <br>

### Les commandes pour l'installation

```
mclovin@mac ~ % /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

mclovin@mac ~ % brew install wget
```

### Les commandes de bases
📒 La documentation ➡️ [https://docs.brew.sh](https://docs.brew.sh)
```
mclovin@mac ~ % brew update
mclovin@mac ~ % brew upgrade
mclovin@mac ~ % brew install
mclovin@mac ~ % brew uninstall
mclovin@mac ~ % brew info
mclovin@mac ~ % brew list
mclovin@mac ~ % brew search
```

<br>

## ![PHP Badge](https://img.shields.io/badge/PHP-777BB4?logo=php&logoColor=fff&style=flat) Installer PHP

### 💻 Chercher les versions de php disponibles à l'installation 

```
mclovin@mac ~ % brew search php
==> Formulae
brew-php-switcher        php-cs-fixer@2           phpbrew                  phpstan
php                      php@7.4                  phplint                  phpunit
php-code-sniffer         php@8.0                  phpmd                    pcp
php-cs-fixer             php@8.1                  phpmyadmin               pup
```
### 💻 Installer la version choisie (php@8.1 pour l'exemple)
```
mclovin@mac ~ % brew install php@8.1
```
### 💡 Info - Répertoire d'installation
```
mclovin@mac ~ % cd /usr/local/etc
mclovin@mac ~ % ls /usr/local/etc
```



<br>

## ![MySQL Badge](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=fff&style=flat) Installer MySQL

### 💻 Installer MySQL
```
mclovin@mac ~ % brew install mysql
```
### Les commandes de bases

📒 La documentation ➡️ [https://formulae.brew.sh/formula/mysql#default](https://formulae.brew.sh/formula/mysql#default)

```
// Se connectter avec l'utilisateur root 
mclovin@mac ~ % bmysql -u root -p

// Charger une bdd à partir d'un fichier
mclovin@mac ~ % mysql -u root -p nom_de_la_base_de_donnees < nom_du_fichier.sql
```