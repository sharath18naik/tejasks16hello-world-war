1 changed file with 22 additions and 0 deletions.
 22  
Jenkinsfile
@@ -0,0 +1,22 @@
pipeline {
    agent any
    stages {
        stage('clone step') {
            steps {
                sh 'rm -rf hello-world-war'
                sh 'git clone https://github.com/venkibiligere/hello-world-war.git'
            }
        }
  stage('Build') {
            steps {
                sh 'mvn package'
            }
  }
//       stage('Deploy step') {
//             steps {
//                 sh 'sudo cp /var/lib/jenkins/${job_name}/hello-world-war-1.0.0.war /var/lib/tomcat9/webapps'      
//             }
//         }
    }
}
