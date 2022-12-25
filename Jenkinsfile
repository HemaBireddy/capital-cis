pipeline {
  agent {label 'linux-slave'}
    stages {
        stage('---clean---') { 
		tools {
			maven 'maven3.8.6'
		}
            steps {
                sh 'mvn clean'
            }
        }
  stage('---test---') { 
		tools {
			maven 'maven3.8.6'
		}
            steps {
                sh 'mvn test'
            }
       }
    }
}
