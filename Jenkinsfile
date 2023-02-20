pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c PES1UG20CS393.cpp'
                sh 'g++ -o PES1UG20CS408 PES1UG20C393.cpp'
                echo 'build stage successfull'
            }
        }
        stage('Test'){
            steps{
                sh './PES1UG20CS393'
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
