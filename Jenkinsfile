pipeline {
    agent any
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello World'
            }
       properties([parameters([booleanParam(defaultValue: true, description: '', name: ''), choice(choices: ['TESTING', 'STAGING', 'PRODUCTION'], description: '', name: 'DEPLOY-ENV'), string(defaultValue: '', description: '', name: '', trim: false)]), pipelineTriggers([[$class: 'PeriodicFolderTrigger', interval: '1m']])])
        }
    }
}
