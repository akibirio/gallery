pipeline { 
  agent any
  stages { 
    stage('clone repository') {
      steps { 
        git 'https://github.com/akibirio/gallery.git'
      }
    }
     stage('Build the project') {
      steps { 
        sh 'echo "here we will Build"'
      }
    }
    stage('Tests') {
      steps { 
        sh 'echo "here we will run tests"'
      }
    }
	stage('Deploy Application') {
      steps { 
        sh 'echo "here I will Deploy to Heroku"'
      }
    }
  }
}