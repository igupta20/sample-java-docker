node {
  agent default
  stage('Build'){
    // build code
  }

  post{
    success {
        echo 'Project build successfully!'
    }
    failure {
        echo 'Project build failed!'
    }
  }  
}