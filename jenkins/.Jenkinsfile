pipeline {
    agent none
    stages {
        stage('Build') {
            agent {
                docker {
                    image 'python:2-alpline'
                }
            }
            steps {
                sh 'python -m py_complie sources/add2vals.py'
            }
        }
    }
}