pipeline {
    agent any
    tools {
        maven "mavenV3_9"
    }
    stages{
        stage("checkout"){
            steps{
                git branch: "main",
                url: "https://github.com/sebastiancalvache/SpringRESTful.git"
            }            
        }
        stage("build"){
            steps{
                sh "mvn compile"
            }
        }
        stage("test"){
            steps{
                sh "mvn test"
            }
        }

    }
}
