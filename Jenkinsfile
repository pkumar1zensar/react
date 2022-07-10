pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                sh "sudo npm install -g --unsafe-perm=true --allow-root"
            }
        }
        stage("Deploy") {
            steps {
                sh "sudo rm -rf /var/www/jenkins-react-app"
                sh "sudo cp -r ${WORKSPACE}/build/ /var/www/jenkins-react-app/"
            }
        }
    }
}
