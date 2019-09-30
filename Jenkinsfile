pipeline {
  agent any
  stages {
    stage('Build') {

        steps {
		  echo 'Building6..'
		  - /usr/local/docker/data/apache-maven-3.5.3/bin/mvn clean package
						
			
        }


    }
    stage('Test') {
      steps {
        echo 'Testing5..'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying5....'
      }
    }
  }
}