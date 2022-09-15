pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build finish'
      }
    }

    stage('test1') {
      parallel {
        stage('test1') {
          steps {
            echo 'test1 is finished'
          }
        }

        stage('test2') {
          steps {
            echo 'test2 complete'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deployed project'
      }
    }

  }
}