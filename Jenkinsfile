pipeline {
    agent {
      label "sibadak"
    }

    stages {
        stage('Say Hello World') {
            steps {
                container("jnlp") {
                    echo "Hello World!"
                }
            }
        }
    }
}
