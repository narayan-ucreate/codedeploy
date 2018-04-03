node {
    stage("install_dependency") {
        sh 'apt-get update'
        sh 'apt-get install -y  software-properties-common'
        sh 'LC_ALL=C.UTF-8 add-apt-repository -y ppa:ondrej/php'
        sh 'apt-get update'
    }
    stage("composer_install") {
         // Run `composer update` as a shell script
         sh 'composer install'

       }
       stage("phpunit") {
         sh 'vendor/bin/phpunit'
      }
}