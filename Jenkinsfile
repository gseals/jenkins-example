pipeline {
    agent any
    
    stages {
        stage ('Compile Stage') {
            steps {
            withMaven(maven : 'mvn3') {
                echo 'mvn clean compile'
                }
            }
        }
        stage ('Testing Stage') {
            steps {
            withMaven(maven : 'mvn3') {
                echo 'mvn test'
                }
            }
        }
        stage ('Deploy Stage') {
                steps {
            withMaven(maven : 'mvn3') {
                echo 'mvn deploy'
                }
            }
        }
    }
}
