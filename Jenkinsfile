pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES2UG20CS506-1 hello.cpp'
                echo "Build Successful"
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG20CS466-1'
            }
        }
        stage('Deploy') {
            steps {
                // deployment code
//                 sh 'cp PES2UG20CS506-1 ../'
                echo 'deployment successful'
            }
        }
    }
    post {
        always {
            echo 'Pipeline completed'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
