pipeline {
    agent any
    tools {
        maven 'maven'
    }
      stages {
        stage('Build') {
            steps {
                // Build your JAR file here
                // For example, using Maven
                sh 'mvn clean package'
            }
        }
        
        // stage("Jar file transfer"){
        //     steps{
        //         sh """echo 'admin123' | sudo -S mv /var/lib/jenkins/workspace/cicd/target/examportal-0.0.1-SNAPSHOT.jar /home/ubuntu/project/"""
        //         sh """echo 'admin123' | sudo -S mv /home/ubuntu/project/examportal-0.0.1-SNAPSHOT.jar /home/ubuntu/project/examportal.jar"""
        //         sh """echo 'admin123' | sudo -S chmod 777 /home/ubuntu/project/examportal.jar"""
        //         // sh "admin123' | sudo -S ls"
        //     }
        // }
        // stage("Running jar file"){
        //     steps{
        //         // sh 'sudo java -jar /home/ubuntu/project/examportal.jar'
        //         // sh """echo 'admin123' | -S systemctl enable examportal"""
        //         // sh """echo 'admin123' | -S systemctl start examportal"""
        //         sh """sudo systemctl enable examportal"""
        //         sh """sudo systemctl start examportal"""
        //         sh """sudo systemctl restart examportal"""
        //         // sh 'sudo cd /home/ubuntu/project'
        //         // sh 'sudo java -jar /home/ubuntu/project/examportal.jar'
        //     }
        // }
        stage(Angular Build){
          steps{
            sh """ng build"""
          }
    }
}