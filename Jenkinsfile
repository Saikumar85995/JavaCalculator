pipeline {
    agent any

    stages {
        stage('Validate') {
            steps {
                echo 'Validating code..'
              sh "/usr/share/maven/bin/mvn validate"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing code..'
              sh "/usr/share/maven/bin/mvn test"
            }
        }
        stage('Build') {
            steps {
                echo 'Building Code....'
              sh "/usr/share/maven/bin/mvn package"
            }
        }
    }
}
