pipeline {
    agent {
        kubernetes {
                label "abc-test"
               defaultContainer 'jnlp'
        }
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
