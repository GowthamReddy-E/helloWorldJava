pipeline {
    agent { label 'one' }  // Restrict the job to run on a node with the specified label

    stages {
      //   stage('Check out') {
        //   steps {
          //    echo "checkOut into the github and clone"
            //  git credentialsId: 'GITHUB', url: 'https://github.com/GowthamReddy-E/helloWorldJava.git'
        //    }
       // }
        stage('clean') {
            steps {
                echo 'Building...'
                sh 'mvn clean'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'mvn clean test'
            }
        }
         stage('Build') {
            steps {
                echo 'Building...'
                sh 'mvn clean install'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
