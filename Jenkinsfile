node {
    stage("install_dependency") {
        //sh 'sudo apt-get update'
        //sh 'sudo apt-get install -y  software-properties-common'
        //sh 'sudo LC_ALL=C.UTF-8 add-apt-repository -y ppa:ondrej/php'
        //sh 'sudo apt-get update'
        //sh 'sudo apt-get install -y php7.0'
        //sh 'sudo apt-get install -y php7.0-ldap'
        //sh 'sudo apt-get install -y php7.0-xml'
        //sh 'sudo apt-get install -y php7.0-xmlrpc'
        //sh 'sudo apt-get install -y php7.0-zip'
        //sh 'sudo apt-get install -y php7.0-mysql'
        //sh 'sudo apt-get install -y php7.0-mbstring'
        //sh 'sudo apt-get install -y php7.0-mcrypt'
        //sh 'sudo apt-get install -y php7.0-gd'
        //sh 'sudo apt-get install -y php7.0-readline'
        //sh 'sudo apt-get install -y php7.0-opcache'
        //sh 'sudo apt-get install -y php7.0-xdebug'
        //sh 'sudo apt-get install -y php7.0-dom'
        //sh 'sudo apt-get install -y php-xdebug'
        //sh 'sudo apt-get install -y php7.0-curl'
        //sh 'sudo apt-get install -y unzip'
       // sh 'wget -nc "http://getcomposer.org/composer.phar"'
        //sh "sudo mv composer.phar /usr/local/bin/composer"
        //sh 'php -r copy("https://getcomposer.org/installer", "composer-setup.php")'
        //sh "php composer-setup.php"
        //sh "php -r unlink('composer-setup.php')"

        
        //sh "mv composer.phar /usr/local/bin/composer"

    }
    stage("composer_install") {
         // Run `composer update` as a shell script
         sh 'sudo composer install'

       }
       stage("phpunit") {
         sh 'vendor/bin/phpunit'
      }
}