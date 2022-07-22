pipeline {
    agent any

    stages {

        stage('Test') {
            steps {
                
                sh "mvn test"
                echo "Webhook Test 2"

            }

            post {
                always {
                    junit '**/target/surefire-reports/TEST-*.xml'
                }
            }
        }

     
        
    }
}
