node {
    stage("install_dependency") {
        sh 'sudo apt-get update'
        sh 'sudo apt-get install -y  software-properties-common'
        sh 'sudo LC_ALL=C.UTF-8 add-apt-repository -y ppa:ondrej/php'
        sh 'sudo apt-get update'
        sh 'sudo apt-get install -y php7.0'
        sh 'sudo php7.0-xml'
        sh 'php7.0-xmlrpc'
        sh 'sudo php7.0-zip'
        sh 'sudo php7.0-mysql'
        sh 'sudo php7.0-mbstring'
        sh 'sudo php7.0-mcrypt'
        sh 'sudo php7.0-gd'
        sh 'sudo php7.0-readline'
        sh 'sudo php7.0-opcache'
        sh 'sudo php7.0-xdebug'
        sh 'sudo php7.0-dom'
        sh 'sudo php-xdebug'
        sh 'sudo php7.0-curl'
        sh 'sudo unzip'
        sh "php -r copy('https://getcomposer.org/installer', 'composer-setup.php')"
        sh "php composer-setup.php"
        sh "php -r unlink('composer-setup.php')"
        sh "mv composer.phar /usr/local/bin/composer"

    }
    stage("composer_install") {
         // Run `composer update` as a shell script
         sh 'composer install'

       }
       stage("phpunit") {
         sh 'vendor/bin/phpunit'
      }
}