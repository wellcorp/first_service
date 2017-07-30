properties([pipelineTriggers([[$class: 'GitHubPushTrigger']])])

node {
    git url: "https://github.com/wellcorp/pwa",
        credentialsId: '04f1e883-0a73-483f-af9b-e38f96bb946e'

    stage("Build") {
        print("Building")
    }
    
    stage("Test") {
        print("Testing")
    }
    
    stage("Deploy Canary") {
        print("Deploying Canary")
    }
    
    stage("Test Canary") {
        print("Testing Canary")
    }
    
    stage("Human Testing") {
        input(message: 'Manual testing succeeded?', ok: 'Yes')
    }
    
    stage("Deploy Production") {
        print("Deploying Production")
    }
}
