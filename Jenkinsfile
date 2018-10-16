pipeline{
    agent any
    stages{
        stage('Install dependencies'){
            steps{
                bat 'npm install'
            }
            post{
                success{
                    echo 'Dependencies successfully installed.'
                }
                failure{
                    echo 'Installation failed!'
                }
            }
        }
        stage('Build'){
            steps{
                bat 'npm run build --prod'
            }
            post{
                success{
                    echo 'App successfully built.'
                }
                failure{
                    echo 'Build failed!'
                }
            }
        }
    }
}