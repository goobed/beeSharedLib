pipeline {
    agent any

    triggers {
        githubPush()
    }

    stages {
        stage('Branch Deletion Event') {
            when {
                expression { currentBuild.rawBuild.getCause("org.jenkinsci.plugins.github.webhook.GHEventPayload$BranchDeleted") != null }
            }
            steps {
                script {
                    def deletedBranch = currentBuild.rawBuild.getCause("org.jenkinsci.plugins.github.webhook.GHEventPayload$BranchDeleted").getRef()
                    echo "Deleted Branch: ${deletedBranch}"
                    
                    // Add your further steps here based on the deleted branch
                }
            }
        }
        // Add more stages for other build events if needed
    }
}
