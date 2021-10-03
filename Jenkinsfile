pipeline {
    agent any
    
    stages {
        stage('Clone repo') {
            steps {
                echo 'Building..'
                git credentialsId: '202104-versent-personal', url: 'https://github.com/alcoholly7/sort_urls.git'
            }
        }
        stage('Run script') {
            steps {
                sh 'ls -la'
                // sh 'python sort_urls.py "https://raw.githubusercontent.com/elastic/examples/master/Common%20Data%20Formats/apache_logs/apache_logs"'
            }
        }
    }
}


