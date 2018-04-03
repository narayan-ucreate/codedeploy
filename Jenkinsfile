node {
    stage("install_dependency") {
        sh 'sudo apt-get update'
        sh 'sudo apt-get install -y  software-properties-common'
        sh 'sudo LC_ALL=C.UTF-8 add-apt-repository -y ppa:ondrej/php'
        sh 'sudo apt-get update'
    }
    stage("composer_install") {
         // Run `composer update` as a shell script
         sh 'composer install'

       }
       stage("phpunit") {
         sh 'vendor/bin/phpunit'
      }
}