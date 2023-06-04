pipeline {
    agent any

    environment { 
        env = credentials('madan')
    }
    stages {
        stage('Hello') {
            steps {
                sh 'printenv'
        }
    }
}
}
