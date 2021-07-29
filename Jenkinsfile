pipeline{
    agent any
    stages{
        stage("A"){
            steps{
                echo "========executing A========"
                powershell 'Write-Host "Hello, Groovy !!!"'
                git branch: 'eesof-develop', credentialsId: '989298a3-fbc0-4c67-b1a1-b4b85c793ac7', url: 'ssh://git@atsbbmirror05.ggn.is.keysight.com:7999/bitbucket/eesof/desjenkins.git'
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
