pipeline{
    agent any 
    stages {
        stage('Init'){
            steps{
                sh "whoami >> output.txt"
                sh "uname -a >> output.txt"
            }
        }
        stage('Intermediate'){
            sh './second_script.sh >> output.txt'
        }
    }
    post {
        success {
                archiveArtifacts artifacts: 'output.txt', followSymlinks: false
            }
        }
}