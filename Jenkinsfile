@Library('mule-lib') _

pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh 'mvn clean -DskipTests package'
            }
        }
        
        stage('Deploy') { 
            steps {
                armDeploy("KrishnaCnK4","T9056#cs","Invenio Solutions","Sandbox","MuleServer","EditX-api","c:\\editxtest-1.0.0-SNAPSHOT-mule-application.jar")
            }
        }
    }
}


// Current version of application is 1.0.BUILD_NBR where BUILD_NBR is provided by Jenkins

