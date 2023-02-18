pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c PES1UG20CS656.cpp'
                sh 'g++ -o PES1UG20CS656 PES1UG20CS656.cpp'
                echo 'BUILD STAGE SUCCESSFUL'
            }
        }
        stage('Test'){
            steps{
                sh './PES1UG20CS656'
                echo 'TEST STAGE SUCCESSFUL'
            }
        }
        stage('Deploy'){
            steps{
                echo 'DEPLOYED SUCCESSFUL'
            }
        }
    }
    post{
        failure{
            echo 'PIPELINE FAILED'
        }
    }
}
