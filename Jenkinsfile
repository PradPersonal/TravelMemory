pipelinne {
  agent {label 'jenkins-agent'}
  stage('Checkout') {
    steps {
      git branch: 'main', url: 'https://github.com/PradPersonal/TravelMemory.git'
    }
  }
  stage('Install') {
    steps {
      sh 'cd backend; npm install'
    }
  }
  stage('Build') {
    steps {
      sh 'cd backend; npm run build'
    }
  }
}
