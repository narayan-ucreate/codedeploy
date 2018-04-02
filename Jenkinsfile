node {
    stage("composer_install") {
         // Run `composer update` as a shell script
         sh 'composer install'
            echo  "done."

       }
       stage("phpunit") {
         sh 'vendor/bin/phpunit'
      }
}