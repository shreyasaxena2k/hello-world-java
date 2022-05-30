pipeline {
    agent any
    // tools {
    //     maven "MAVEN"
    // }
    stages{
        stage("Clone code from GitHub") {
            steps {
                script {
                    git branch: "master", credentialsId: 'github_cred', url: "https://github.com/shreyasaxena2k/hello-world-java";
                }
            }
        }
        stage('Build'){
            steps{
                 sh script: 'mvn clean package'
            }
        }

    }
}



