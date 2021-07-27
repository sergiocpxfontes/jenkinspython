pipeline {
    //agent any
    agent {
        label 'SergioOC'
    }
    stages {
        stage('build') {
          steps {
            //sh 'pip install -r requirements.txt'
              echo "sergio"
          }
        }
        stage ('Test'){
            steps {
                sh 'python PythonApplication1/PythonApplication1/test-app.py'
            }
        }
    }
}
