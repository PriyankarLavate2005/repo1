pipeline {
    agent any
    stages {
        stage('hello') {
            steps {
                script {
                    echo 'hello Priyanka'
                    echo "hello Pooja how are you"

                }
            }
        }
        stage('Take approval'){
            steps{
                timeout(time:1,unit:minutes){
                    input message :"do you want to procced" ,ok='procced'
                }
            }
        }
    }
}
