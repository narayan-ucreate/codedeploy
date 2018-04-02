node {
    stage("composer_install") {
         // Run `composer update` as a shell script
         sh 'composer install'

              echo  "this is env variable ${env.BUILD_ID}"

       }
       stage("phpunit") {
         sh 'vendor/bin/phpunit'
      }
}