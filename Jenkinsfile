pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo "Its Building the Code"
            }
        }
        stage('Test') { 
            steps {
                echo "Its Testing the Code"
            }
        }
        stage('Deploy') { 
            steps {
                input 'Does the staging environment look OK?'
                milestone(1)
                echo "Its Deploying the Code"
            }
        }
    }
}
