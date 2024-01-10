pipeline {
    agent any
    parameters {
        string(name: 'MYNAME', defaultValue: 'Mubin', description: 'Plz enter your name')
        string(name: 'MYSURNAME', defaultValue: 'Maniyar', description: 'Plz enter your surname')
        booleanParam(name: 'CHOICE', defaultValue: true, description: 'Plz provide choice')
    }
    stages {
        stage('Build') {
            steps {
                sh 'chmod +X ./name.sh'
                sh './esmail.sh ${params.MYNAME} ${params.MYSURNAME}'
            }
        }


    }
}
