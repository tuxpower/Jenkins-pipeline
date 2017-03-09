pipeline {
    agent any
    input message: 'XYZ', parameters: [choice(choices: ['LIST', 'ADD', 'DELETE'], description: 'Choose from one of the 3 functions LIST, ADD, DELETE.', name: 'Options')]
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
