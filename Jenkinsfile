pipeline{
    agent any
    environment{
        PATH= "/opt/maven/bin:$PATH"
    }
    stages{
        stage('git clone'){
            steps{
                 git url: 'https://github.com/Jinendra-b-1008/war-web-project.git' , branch: 'master'
            }
        }
        stage('build'){
            steps{
                sh 'mvn clean install'
            }
        }
    }
}
