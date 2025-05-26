pipeline {
    agent any 

    stages {
        stage('Deploy') {
            steps {
              echo 'Publishing HTML'
                publishHTML(target: [
                    reportDir: '.',
                    reportFiles: 'index.html',
                    reportName: 'Build Report',
                    allowMissing: false,
                    alwaysLinkToLastBuild: true,
                    keepAll: true
                ])
            }
        }
    }
}
