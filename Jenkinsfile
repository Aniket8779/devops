pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
         git branch: 'main',url: 'https://github.com/Aniket8779/devops.git'
            }
          }
    stage('Deploy to apache') {
       steps {
         sh "
             sudo rm -rf /var/www/html/*
             sudo cp -r * /var/www/html/
             sudo chown -R www-data:www-data /var/www/html
             "
              }
       }
    }
}
