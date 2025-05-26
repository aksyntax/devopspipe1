pipeline {
    agent any 

    stages {
        stage('Deploy') {
            steps {
                git branch: 'main', url:'https://github.com/aksyntax/devopspipe1.git'
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
