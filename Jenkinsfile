pipeline {
  agent {
    label 'ubuntu'
  }
     stages {
        stage('Build') {
            agent {
                docker {
                    image 'sebp/elk'
                    // Run the container on the node specified at the
                    // top-level of the Pipeline, in the same workspace,
                    // rather than on a new node entirely:
                    reuseNode true
                }
            }
        }
     }
}
