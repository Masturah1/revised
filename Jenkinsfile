pipeline{
    agent any
    stages{
        stage("Test"){
            steps{
                sh '''
                       echo "Hello World"
                   '''
            }
        }
        stage("Build"){
            steps{
                sh '''
                      ## Get the project


                      touch index.html
                      


                       sudo docker build -t masturrh/pixer:latest .

                       sudo docker run -d -p 801:80 masturrh/pixer:latest
                   
                   
                   
                   '''
            }
        }
    }
}