// pipeline {
//  agent any {
//     stages {

//     stage('Build') {
//        echo " Build "
//     }
//     stage('Test') {
//          echo " TEST "
//     }
//     stage('Deploy') {
//        echo " Deploy "
//     }
//         }

//  }
  
// }


pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Hello, build!'
            }
        }
        stage('Test') {
            steps {
                echo 'Hi, test!'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Hey, Deploy!'
            }
        }
    }
}