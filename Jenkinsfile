pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                               sh """
                    echo ${SHELL}
                    [ -d venv ] && rm -rf venv
                    #virtualenv --python=python2.7 venv
                    virtualenv venv
                    #. venv/bin/activate
                    export PATH=${VIRTUAL_ENV}/bin:${PATH}
                    pip install -r requirements.txt 
                """
            }
        }
    }
}
