pipeline {
agent any
stages {
    
    /*
    stage ('GIT Checkout'){
        steps {
            git changelog: false, poll: false, url: 'https://github.com/Tasfiq23/Devops_assessment_2.git'
        }
    }
    */
    stage('build') {
      steps {
        //sh 'pip install -r requirements.txt'
      }
    }
    stage ('Test'){
        steps {
            sh 'python unit-test.py'
        }
    }
}
}
