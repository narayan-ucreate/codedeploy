node {
    stage("composer_install") {
         // Run `composer update` as a shell script
         sh 'composer install'
echo sh(returnStdout: true, script: 'env')
             // echo  "this is env variable ${env.JOB_NAME}
       }
       stage("phpunit") {
         sh 'vendor/bin/phpunit'
      }
}