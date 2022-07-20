pipeline { 
  agent any
  tools{
	nodejs 'Node-14'
  }
  
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
	stage('Install Dependencies') {
      steps { 
        sh 'npn install"'
      }
    }
    stage('Tests') {
      steps { 
        sh 'npm test"'
      }
    }
	stage('Deploy Application') {
      steps { 
        sh 'echo "here I will Deploy to Heroku"'
      }
    }
  }
}