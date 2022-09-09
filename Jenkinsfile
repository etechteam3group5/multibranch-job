pipeline {
    agent any
    stages{
        stage('system statistics and Jenkins status check'){
            parallel{
                stage('Max'){
                    steps{
                        sh "lscpu"
                         sh "sudo systemctl status jenkins"
                    }
                }
                stage('Chima'){
                    steps{
                        sh "lscpu"
                        sh "sudo systemctl status jenkins"
                    }
                }
            }
            parallel{
                stage('Christiana'){
                    steps{
                        sh "lscpu"
                         sh "sudo systemctl status jenkins"
                    }
                }
                stage('Tunde'){
                    steps{
                        sh "lscpu"
                        sh "sudo systemctl status jenkins"
                    }
                }
            }
        }
        stage('End of parallel build'){
            steps{
                echo "End of multi-branch-build pipeline"
            }
        }
    }
}
