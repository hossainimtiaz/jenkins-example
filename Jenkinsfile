pipeline {
    agent any

    tools {
        maven 'Maven 3.3.9'
        jdk 'jdk8'
    }

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven() {
                    sh 'mvn clean compile'
                }
            }
        }
    }
}