pipeline {
  agent any
  stages {
    stage('Source') { 
      steps {
			// Some Step
	   checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'git@github.com:neelam7/jenkins2-course-spring-boot.git']]])
      }
    }
    stage('Compile') { 
      tools {
        // Specify Tool Name from your global tool configuration
		jdk 'JDK'
        maven 'Maven'
      }
      steps {
			// Some Step
      }
    }
  }
}
