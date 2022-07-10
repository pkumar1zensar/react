pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                 echo 'building....'
                sh "sudo npm install"
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
