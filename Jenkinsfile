
pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                 sh 'pip install requirements.txt'
                 sh 'python app.py' 
            }
        }
    }
}
