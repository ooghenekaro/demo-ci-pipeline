pipeline {
    agent any
    
    stages {
        stage('valdiate') {
            steps {
                echo 'mvn clean package'
            }
        }
        stage('test') {
            steps {
              echo 'mvn test'
            }
        }
      stage('Build') {
            steps {
              echo 'mvn clean install'
            }
        }
    }
    
    post {
        success {
            // Actions to perform if the build is successful
            echo 'Build successful!'
        }
        failure {
            // Actions to perform if the build fails
            echo 'Build failed!'
        }
    }
}
