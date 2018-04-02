node {
    stage("composer_install") {
         // Run `composer update` as a shell script
         sh 'composer install'
            echo  "this is env variable${env.APP_NAME}"
              echo  "this is env variable${APP_NAME}"

       }
       stage("phpunit") {
         sh 'vendor/bin/phpunit'
      }
}