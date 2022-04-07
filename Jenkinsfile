pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'echo "Hello World"'
                bat '''
                    echo "Multiline shell steps works too"
                '''
            }
        }
    }
    post {
        always {
        archiveArtifacts artifacts: 'demofile', followSymlinks: false
        }
    }
}
