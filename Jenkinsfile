pipeline {
  agent {
    kubernetes {
    }
  }

    node(POD_LABEL) {
                stage('Shell Execution') {
                    sh '''
                    echo "Hello! I am executing shell"
                    '''
                }
        }

}
