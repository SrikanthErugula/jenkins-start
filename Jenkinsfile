pipeline {
    agent {
        node {
            label 'AGENT-1'
        }
    }
    environment{
        COURSE = "Jenkins with DEVOPS"
    }
    stages {
        stage('Build') {
            steps {
                script{
                    sh """
                        echo 'Hello, Building!'
                        echo $COURSE
                        env
                    """
                }
                
            }
        }
        stage('Test') {
            steps {
                script{
                    sh """
                        echo 'Hello, Testing !'
                        echo $COURSE
                    """
                }
            }
        }
        stage('Deploy') {
            steps {
                script{
                    sh """
                        echo 'Hello, Deploying!'
                        env
                    """
                }
            }
        }
    }
    post{  
        always{
            echo 'I will always say Hello again!'
            cleanWs()
        }
        success {
            echo 'I will run if success'
        }
        failure {
            echo 'I will run if failure'
        }
//         aborted {
//             echo 'pipeline is aborted'
//         }
    }
}