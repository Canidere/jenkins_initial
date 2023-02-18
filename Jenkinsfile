pipeline{
    agent any 
    stages {
        stage('Init'){
            steps{
                echo "whoami >> output.txt"
                sh "uname -a >> output.txt"
            }
        }
    }
}