import java.util.concurrent.TimeUnit

pipeline {
    agent any
    stages {
        stage('hello') {
            steps {
                script {
                    echo 'hello Priyanka'
                    echo 'hello Pooja, how are you?'
                }
            }
        }
        stage('Take approval'){
            steps{
                timeout(time: 1, unit: TimeUnit.MINUTES) {
                    input message: 'Do you want to proceed?', ok: 'Proceed'
                }
            }
        }
    }
}
