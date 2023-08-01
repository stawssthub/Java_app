 @Library('my_shared_library') _

pipeline {

    agent any
    tools {
        maven 'maven-3.9'
    }
    stages{
        stage('git checkout'){
            steps {
               // checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/stawssthub/Java_app.git']])
               //git branch: 'main', url: 'https://github.com/stawssthub/Java_app.git'

                 
                script{
                  gitCheckout{
                     branch: "main"
                     url: "https://github.com/stawssthub/Java_app.git"
               }
            }
            }
        }
    }
}