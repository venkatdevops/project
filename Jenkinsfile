pipeline {
    agent any

    stages {
        stage ('Clean ') {

            steps {
                withMaven(maven : 'mvn') {
                    sh 'mvn clean'
                }
            }
        }

        stage ('complie') {

            steps {
                withMaven(maven : 'mvn') {
                    sh 'mvn compile'
                }
            }
        }


        stage ('install') {
            steps {
                withMaven(maven : 'mvn') {
                    sh 'mvn install'
                }
            }
        }
    }
}
