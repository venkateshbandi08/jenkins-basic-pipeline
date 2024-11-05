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
        stage('Create and Write File') {
            steps {
                // Using PowerShell script in Jenkins
                powershell '''
                    # Define the file path and content
                    $filePath = "output.txt"
                    $content = "Hello, this is a sample text written to the file."

                    # Create the file and write content to it
                    Set-Content -Path $filePath -Value $content

                    # Print the content of the file
                    Get-Content -Path $filePath
                '''
            }
        }
    }
}
