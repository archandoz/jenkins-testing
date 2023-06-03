pipeline {

    stages {
        stage('Cloning Git') {
            steps {
                script {
                    checkout([
                        $class: 'GitSCM',
                        branches: [[name: 'refs/heads/master']],
                        extensions: [[$class: 'CloneOption', noTags: false, shallow: false, depth: 0, reference: '']],
                        userRemoteConfigs: scm.userRemoteConfigs,
                    ])
                }
            }
        }

        stage('ddd Git') {
            steps {
                script {
                    echo 'vvvv'
                }
            }
        }


    }
}
