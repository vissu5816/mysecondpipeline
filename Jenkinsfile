pipeline {
  agent any
  stages {
    stage('ci') {
      parallel {
        stage('ci') {
          steps {
            git(url: 'https://VISHWANATHREDDY.K%40thermofisher.com@stash.amer.thermo.com/scm/icma/icma-android.git', poll: true)
          }
        }
        stage('build') {
          steps {
            sh '''echo "Building dev apk file"
./gradlew -i app:assembleDevDebug'''
          }
        }
      }
    }
  }
}