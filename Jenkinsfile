pipeline {
  agent {
    node { label 'workstation'}
  }

  stages {

    stage('Build ') {
          steps {
            echo 'Build'
          }
    }

    stage('Unit Test ') {
          steps {
            echo 'Unit Test'
           // sh 'python -m unittest'
          }
    }

    stage('Code Analysis ') {
          steps {
            sh 'sonar-scanner -Dsonar.host.url=http://18.215.243.239:9000 -Dsonar.login=admin -Dsonar.password=admin123 -Dsonar.projectKey=payment'
          }
    }

    stage('Security scan ') {
          steps {
            echo 'Security scan'
          }
    }
    
    stage('Publish Artifact ') {
          steps {
            echo 'Publish Artifact'
          }
    }

  }

}