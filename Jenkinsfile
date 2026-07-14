pipeline {
     agent any

     stages {
      stage('clone code'){
        steps {
          git 'https://github.com/hrithik-k0/DevOps-project.git'
        }

      }

      stage('Build Docker Image') {
        steps {
          sh 'docker build -t hk00d/devops-app .'
        }
      }

      stage('push to DockerHub') {
        steps {
          sh 'docker push hk00d/devops-app'
        }
      }
     }
}