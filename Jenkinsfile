pipeline {
  agent any
  
       tools {
        //工具名称必须在Jenkins 管理Jenkins → 全局工具配置中预配置。
        maven 'maven-3.5.0'
    }
  stages {
    stage('Build') {

        steps {		
		  compileAllFiles()			
			
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


	def compileAllFiles()
	{
		//执行shell命令
		//sh 'mvn -f /var/jenkins_home/workspace/springboot-seckill2_master/pom.xml clean install -DskipTests=true'
		sh 'mvn -f /var/jenkins_home/workspace/springboot-seckill2_master/pom.xml clean  package  -DskipTests=true'
	}