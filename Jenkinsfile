pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c PES1UG20CS144.cpp'
                sh 'g++ -o PES1UG20CS144 PES1UG20CS144.cpp'
                echo 'build stage successfullllllll'
            }
        }
        stage('Test'){
            steps{
                sh './PES1UG20CS144'
                echo 'Test stage executed successfully'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deployed Successfully'
            }
        }
    }
    post{
        failure{
            echo 'Pipeline Failed'
        }
    }
}
