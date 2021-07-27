pipeline {
    agent any
    stages {
        stage('build') {
          steps {
            //sh 'pip install -r requirements.txt'
              echo sergio
          }
        }
        stage ('Test'){
            steps {
                sh 'python test-app.py'
            }
        }
    }
}
