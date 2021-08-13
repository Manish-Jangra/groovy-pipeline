pipeline{
    agent {
    label "slmo-win10-03"}
    stages{
        stage("A"){
            steps{
                echo "========executing A========"
                powershell 'Write-Host "Hello, Manish !!!"'
            }
            post{
                always{
                    echo "========always========"
                    powershell 'Write-Host "Hello, Manish !!!"'
                }
                success{
                    echo "========A executed successfully========"
                    powershell 'Write-Host "Hello, Manish !!!"'
                }
                failure{
                    echo "========A execution failed========"
                    powershell 'Write-Host "Hello, Manish !!!"'
                }
            }
        }
    }
    post{
        always{
            echo "========always========"
            powershell 'Write-Host "Hello, Manish !!!"'
        }
        success{
            echo "========pipeline executed successfully ========"
            powershell 'Write-Host "Hello, Manish !!!"'
        }
        failure{
            echo "========pipeline execution failed========"
            powershell 'Write-Host "Hello, Groovy !!!"'
        }
    }
}
