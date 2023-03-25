agent {
	kubernetes {
		inheritFrom 'jenkins-jenkins-agent'
	}
environment {
    CONTAINER_ENV_VAR = 'container-env-var-value'
  }
  stages {
    stage('Run maven') {
      steps {
        sh "echo OUTSIDE_CONTAINER_ENV_VAR = ${CONTAINER_ENV_VAR}"

      }
    }
	stage('Run maven with a different shell') {
		steps {
			sh 'mvn -version'
		}
	  }
  }	
}
