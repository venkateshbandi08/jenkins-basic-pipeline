pipeline {
    agent {
        label 'jenkinsagent'
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage("Dev"){
            steps{
                echo "Dev stage"
            }
        }
        stage("Test"){
            steps{
                echo "Test stage"
            }
        }
        stage("QA"){
            steps{
                echo "QA stage"
            }
        }
        stage("Deploy"){
            steps{
                echo "Deploy stage"
            }
        }
    }
}
