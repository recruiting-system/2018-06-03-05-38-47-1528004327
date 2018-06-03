pipeline {
    agent {
        docker { image 'wannabefro/ruby-rspec' }
    }
    stages {
        stage('Build'){
            steps {
                sh 'echo $quiz > quiz.rb'
                sh 'echo $testData > test-data.json'
                sh 'ls -l'
                sh 'cat quiz.rb'
                sh 'cat test-data.json'
            }
        }
        stage('Test'){
            steps {
                sh 'rspec'
            }
        }
        stage('Save Test Result'){
            steps {
                echo 'Hello world!'
            }
        }
    }
}
