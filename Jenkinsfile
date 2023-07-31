@Library('bee-shared-lib') _

pipeline {
    agent any
    stages {
        stage('Dance Party') {
            steps {
                org.jenkins.beeSharedUtils.danceParty()
            }
        }
        stage('Unleash the Dragons') {
            steps {
                org.jenkins.beeSharedUtils.unleashTheDragons()
            }
        }
        stage('Launch Rocket') {
            steps {
                org.jenkins.beeSharedUtils.launchRocket()
            }
        }
        stage('Deploy to Kubernetes') {
            steps {
                deployToK8s(namespace: 'my-k8s-namespace', deploymentName: 'my-app-deployment')
            }
        }
    }
}
