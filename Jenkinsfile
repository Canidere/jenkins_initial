pipeline{
    agent any 
    stages {
        stage('Init'){
            steps{
                sh "whoami >> output.txt"
                sh "uname -a >> output.txt"
            }
        }
    }
}