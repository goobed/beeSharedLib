@Library('bee-shared-lib') _

pipeline {
    agent any
    stages {
        stage('Dance Party') {
            steps {
                org.jenkins.bee-shared-utils.danceParty()
            }
        }
        stage('Unleash the Dragons') {
            steps {
                org.jenkins.bee-shared-utils.unleashTheDragons()
            }
        }
        stage('Launch Rocket') {
            steps {
                org.jenkins.bee-shared-utils.launchRocket()
            }
        }
        stage('Deploy to Kubernetes') {
            steps {
                deployToK8s(namespace: 'my-k8s-namespace', deploymentName: 'my-app-deployment')
            }
        }
    }
}
