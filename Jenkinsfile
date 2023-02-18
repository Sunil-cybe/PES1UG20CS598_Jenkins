pipeline{
    agent any 
    stages{
        stage('Build')
        {
            steps{
                sh 'g++ -c PES1UG20CS598.cppp'
                sh 'g++ -o PES1UG20CS598 PES1UG20CS598.cpp'
                echo 'Build Done'
            }
        }
        
        stage('Test')
        {
            steps{
                sh './PES1UG20CS598'
                echo 'Test stage done'
            }
        }
        
        stage('Deploy'){
            steps{
                echo 'Deploy done'
            }
        }
        
        
        
    }
    post{
        failure{
            echo 'Pipeline failed'
        }
    }
}
