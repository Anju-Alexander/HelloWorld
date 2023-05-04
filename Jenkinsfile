pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build App'
            }
        }
        stage('Test1') {
            steps {
                echo 'Test App'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy App'
            }
        }
        stage('CheckoutModule1') {
        steps {
                sh 'mkdir -p Module1'
                dir("Module1")
                {
                    git branch: "develop",
                    //credentialsId: 'aaa',
                    url: 'https://github.com/Anju-Alexander/HelloWorld.git'
                }
            }
        }
    }
}
