pipeline{
    agent any
    stages{
        stage("Stage 1 Pull the Java code from repository οefremidis/Quiz2_MathApp"){
            steps{
                git url: 'https://github.com/oefremidis/Quiz2_MathApp.git';
            }
        }
        stage("Stage 2: package the code using maven"){
            steps{
                sh 'mvn package';
            }
        }
        stage("Stage 3: run the code"){

        }
        stage()
    }
    post{
        success {
            echo "Successful project build and run."
        }
        failure {
            echo "Project failure"
        }
    }

}