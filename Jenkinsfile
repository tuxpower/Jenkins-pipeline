pipeline {
    agent any
    parameters {
        string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
    }
    stages {
        stage('English') {
            steps {
                echo "${Greeting} World!"
            }
        }
        stage('Portuguese') {
            steps {
                echo "${Greeting} Mundo!"
            }
        }
    }
}
