pipeline{
    agent any
    
    environment{
        PATH = "/opt/maven/bin${PATH}"
    }

    stages{
        stage('git copied'){
            steps{
                echo 'source code checked by Jenkins file'
            }

        }
        stage('Building') {
            steps{
                sh '''
                pwd
                ls -ltr
                mvn clean package
                '''
            }
        }
    }
}


