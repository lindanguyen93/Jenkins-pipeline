pipeline{

    agent any

    stages{
        stage('Build'){
            steps{
                echo "Building ..."             
            }
            post {
                always{
                    mail to: "linda.work93@gmail.com",
                    subject: "Build Status Email",
                    body: "Build log attached!"
                }
            }     
         }
        stage ("Test") {
            steps {
                echo "testing..."
            }
        }
        stage("Deploy"){
            steps {
                echo "Deploying ..."
            }
        }
    }
}
