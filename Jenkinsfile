pipeline{
    agent any
    stages{
        stage("A"){
            steps{
                echo "========executing A========"
                powershell 'Write-Host "Hello, Manish !!!"'
            }
            post{
                always{
                    echo "========always========"
                    powershell 'Write-Host "Hello, Groovy !!!"'
                }
                success{
                    echo "========A executed successfully========"
                    powershell 'Write-Host "Hello, Groovy !!!"'
                }
                failure{
                    echo "========A execution failed========"
                    powershell 'Write-Host "Hello, Groovy !!!"'
                }
            }
        }
    }
    post{
        always{
            echo "========always========"
            powershell 'Write-Host "Hello, Groovy !!!"'
        }
        success{
            echo "========pipeline executed successfully ========"
            powershell 'Write-Host "Hello, Groovy !!!"'
        }
        failure{
            echo "========pipeline execution failed========"
            powershell 'Write-Host "Hello, Groovy !!!"'
        }
    }
}
