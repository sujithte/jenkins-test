pipeline {
    agent {
        kubernetes {
            yaml '''
apiVersion: v1
kind: Pod
metadata:
  name: andreas-test
spec:
  containers:
  - name: jnlp
    image: jenkins/inbound-agent:latest-jdk17
'''

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
