node {

   // Mark the code checkout 'stage'....

   stage 'Checkout'

   // Get some code from a Bitbucket repository

   git credentialsId: '5239c33e-10ab-4c1b-a4a0-91b96a07955e', url: 'git@bitbucket.org:matthewbdaly/my-app.git'

   // Install dependencies

   stage 'Install dependencies'

   // Run Composer

   sh 'composer install'

   // Test stage

   stage 'Test'

   // Run the tests

   sh "vendor/bin/phpunit"

}