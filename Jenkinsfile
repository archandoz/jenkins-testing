pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                checkout scmGit(branches: [[name: 'refs/heads/develop']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/archandoz/jenkins-testing.git']])            }
        }
    }
}
