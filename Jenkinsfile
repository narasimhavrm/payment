pipeline {
  agent {
    node { label 'workstation'}
  }

  stages {

    stage('Code Checkout ') {
      steps {
        echo 'Code Checkout'
      }
    }

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
            echo 'Code Analysis'
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