Note: MVC - models - manage data views - blade or vue components controller - handle requests using models and views to generate final responses as seen in browsers

### INSTALL PHP8.2
sudo apt update && sudo apt -y upgrade

sudo apt autoremove

[ -f /var/run/reboot-required ] && sudo reboot -f

sudo apt update

sudo apt install -y lsb-release gnupg2 ca-certificates apt-transport-https software-properties-common

sudo add-apt-repository ppa:ondrej/php

sudo apt install php8.2

### INSTALL PHP CURL
sudo apt-get install php-curl

### INSTALL PHP XML
sudo apt-get install php-xml 

### INSTALL COMPOSER
sudo apt install php-cli unzip

curl -sS https://getcomposer.org/installer -o /tmp/composer-setup.php

HASH=`curl -sS https://composer.github.io/installer.sig`
php -r "if (hash_file('SHA384', '/tmp/composer-setup.php') === '$HASH') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"


sudo php /tmp/composer-setup.php --install-dir=/usr/local/bin --filename=composer

### INSTALL LARAVEL EMILLE METHOD
composer create-project --prefer-dist laravel/laravel ./ "10.*" 

## INSTALL NODEJS AND VUE
curl -fsSL https://deb.nodesource.com/setup_19.x | sudo -E bash -

sudo apt install -y nodejs

## INSTALL VITE + VUE [FRONTEND FOLDER]
npm create vite@latest ./

npm install

## INSTALL DOCKER COMPOSE
apt-get install docker-compose

## CREATE FILE FROM COMMAND LINE
touch filename

### TO START OR STOP ENVIRONMENT
docker-compose up
docker-compose down

### RUN LARAVEL SERVER
php artisan serve --host=0.0.0.0 --port=8000

TO CONNECT LARAVEL TO DATABASE
within backend folder update .env database credentials
..................................

TO CREATE CONTROLLER
php artisan make:controller controllerName

CHECK ROUTES
php artisan route:list

## TO CONNECT LARAVEL TO DATABASE
- within backend folder update .env database credentials

### TEST DB CONNECTION
- php artisan tinker
- DB::connection()->getPdo():


### BRAND NEW GIT REPO
- git init
- git remote add origin <repourl>

### TO COMMIT TO GIT HUB
[CD INTO FOLDER]
- git init 
- git add .
- git commit -m "message"
- git push origin <branchName>

### TO PULL FROM GITHUB
- git pull origin <main>

