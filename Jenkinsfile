pipeline {
    agent any
    
    stages {
        stage ("sample page") {
            steps {
                echo "this is sample declarative code"
            }
        }
        
        stage ("check the packages and disk and memory") {
            steps {
                sh "rpm -qa | grep git"
                echo "below is the disk and memory"
                sh "df -h"
                sh "du -ksh"
                sh "free -m"
            }
        }
    }
}
