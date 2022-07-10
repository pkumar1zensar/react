pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                 echo 'building....'
                sh "sudo npm install"
            }
        }
        stages {
        stage("Test") {
            steps {
                 echo 'testing....'
                sh "sudo npm test"
            }
        }
        stage("Deploy") {
            steps {
                 echo 'deploying ....'
                sh "sudo npm run build"
                
            }
        }
    }
}
