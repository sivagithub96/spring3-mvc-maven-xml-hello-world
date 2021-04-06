pipeline {
  agent any
  stages {
    stage('getcode') {
      steps {
        git(url: 'https://github.com/sivagithub96/spring3-mvc-maven-xml-hello-world.git', branch: 'master', changelog: true, poll: true)
      }
    }

    stage('maven') {
      steps {
        sh 'mvn package'
      }
    }

  }
}