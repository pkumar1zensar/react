pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                 echo 'building....'
                sh "sudo npm install -g --unsafe-perm=true --allow-root"
            }
        }
        stage("Deploy") {
            steps {
                 echo 'deploying ....'
                sh "sudo npm start"
                
            }
        }
    }
}
