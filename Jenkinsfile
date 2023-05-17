currentBuild.displayName = "Jenkins Demo "+currentBuild.number
pipeline{
    agent any
    stages{
        stage("Welcome"){
            steps{
                echo "Welcome to Jenkins Declarative pipeline"
            }
        }
        stage("Git Checkout"){
            steps{
                git credentialsId: '9d40eb18-e5e3-4346-a579-f9c8257a8862', url: 'https://github.com/dedeepya2281manne/spring-boot-jenkins'
            }
        }
        stage("Maven Build"){
            steps{
                sh "mvn clean package"
            }
        }
    }
}
