pipeline {
    agent any
    
    stages {
        stage ('Compile Stage') {
            steps {
            withMaven(maven : 'mvn3') {
                bat 'mvn clean compile'
                }
            }
        }
        stage ('Testing Stage') {
            steps {
            withMaven(maven : 'mvn3') {
                bat 'mvn test'
                }
            }
        }
        stage ('Deploy Stage') {
                steps {
            withMaven(maven : 'mvn3') {
                bat 'mvn deploy'
                }
            }
        }
    }
}
