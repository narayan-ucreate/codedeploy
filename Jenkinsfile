node {
    stage("composer_install") {
         // Run `composer update` as a shell script
         sh 'composer install'
  sh 'env > env.txt'
    readFile('env.txt').split("\r?\n").each {
        println it
    }
       }
       stage("phpunit") {
         sh 'vendor/bin/phpunit'
      }
}