pipeline {
    agent any

    parameters {
        string(defaultValue: "master", description: 'Which branch?', name: 'BRANCH_NAME')
    }

    stages {
        stage('test'){
            steps {
                echo  "/jenkins/upload_s3.sh s3://privacera/ranger/ranger-${params.BRANCH_NAME}"
            }
        }
    }
}
