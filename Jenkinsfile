pipeline {
    agent any

    stages {

        stage('Test') {
            steps {
                
                sh "mvn test"
                echo "Webhook Test"

            }

            post {
                always {
                    junit '**/target/surefire-reports/TEST-*.xml'
                }
            }
        }

     
        
    }
}
