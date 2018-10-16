pipeline{
    agent any
    stages{
        stage('Test'){
            steps{
                bat 'ng test'
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