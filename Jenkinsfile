pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c PES1UG20CS598.cpp'
                sh 'g++ -o PES1UG20CS598 PES1UG20CS598.cpp'
                echo 'build stage successfull'
            }
        }
        stage('Test'){
            steps{
                sh './PES1UG20CS598'
                echo 'Test stage executed successfulllllly'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deployed Successfulllllly'
            }
        }
    }
    post{
        failure{
            echo 'Pipeline Failed'
        }
    }
}
