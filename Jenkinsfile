pipeline{
    agent any 
    stages{
      stage('CodeScan'){
        steps{
            sh 'trivy fs . -o results.html'
            sh 'cat result.html'
            
        }
      }
    stage('dockerImageBuild'){
        steps{
            sh 'docker -v'
        }
    }
    stage('pushImage'){
        steps{
            sh 'docker ps'
        }
    }
    }
}