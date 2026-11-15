pipeline{
    agent any
    tools{
        maven 'MAVEN_HOME'
    }
    stages{
        stage('git checkout'){
            steps{
                git branch: 'main',
                url:'https://github.com/madhanijayanthi2805-star/maven_java.git'
            }
        }
        stage('clean'){
            steps{
                bat 'mvn clean'
            }
        }
        stage('install'){
            steps{
                bat 'mvn install'
            }
        }
        stage('test'){
            steps{
                bat 'mvn test'
            }
        }
        stage('package'){
            steps{
                bat 'mvn package'
            }
        }
    }
}
