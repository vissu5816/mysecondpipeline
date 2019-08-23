pipeline {
  agent any
  stages {
    stage('ci') {
      steps {
        git(url: 'https://VISHWANATHREDDY.K%40thermofisher.com@stash.amer.thermo.com/scm/icma/icma-android.git', poll: true)
      }
    }
    stage('build') {
      steps {
        sh '''echo "Building dev apk file"
./gradlew -i app:assembleDevDebug'''
        svn(url: 'https://svn.amer.thermo.com/scm/svn/dhap/mustang-automation/voice-connect', poll: true)
      }
    }
    stage('method') {
      steps {
        jobDsl(scriptText: 'jkvfdjkn')
      }
    }
  }
}