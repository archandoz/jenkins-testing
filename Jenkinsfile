pipeline {
    agent any

    environment { 
        env = 'clang'
    }
    stages {
        stage('Hello') {
            steps {
                echo "MY_TEXT"
                echo  env
        }
    }
}
}
