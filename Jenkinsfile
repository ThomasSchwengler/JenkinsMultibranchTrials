pipeline {
    agent any
    
    triggers {
        issueCommentTrigger('.*test this please.*')
    }

    stages {
        stage("Build") {
            steps {
                sh './build.sh'
                sh './build2.sh'
            }
        }
    }
}
