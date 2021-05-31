pipeline {
    agent any

    tools {
        maven 'Maven 3.3.9'
        jdk 'jdk8'
    }

    stage ('Initialize') {
        steps {
            sh '''
                echo "PATH = ${PATH}"
                echo "M2_HOME = ${M2_HOME}"
            '''
        }
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