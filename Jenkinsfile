pipeline {
    agent any

    environment { 
        env = 'clang'
    }
    stages {
        stage('Hello') {
            steps {
                def now = new Date()
                env.DATE_NOW = now.format("yyyy_MM_dd_HH_mm", TimeZone.getTimeZone('Asia/Bangkok'))

                env.COMMIT_HASH = sh(returnStdout: true, script: "git log -n 1 --pretty=format:'%h'").trim()
                echo "COMMIT_HASH"
                echo env.COMMIT_HASH
                env.REPO_NAME = "lark-adapter"
                env.ENV_UNITTEST_FILE = "./.env-unittest"
                env.AWS_ECR_REP = "502886420734.dkr.ecr.ap-southeast-1.amazonaws.com/${env.REPO_NAME}"

                echo env
        }
    }
}
}
