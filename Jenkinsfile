pipeline{
    agent any
    stages{
        stage('Test'){
            steps{
                bat 'npm install'
                bat 'npm test'
            }
            post{
                success{
                    echo 'App successfully tested.'
                }
                failure{
                    echo 'Tests failed!'
                }
            }
        }
    }
}