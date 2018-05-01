pipeline {
    agent any

    stages {
        stage ('Package Stage') {

            steps {
                withMaven(maven : 'M3') {
                    bat 'mvn clean package'
                }
            }
        }



        stage ('Deployment Stage') {
            steps {
                withMaven(maven : 'M3') {
                    bat 'mvn deploy'
                }
            }
        }
    }
}
