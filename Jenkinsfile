pipeline {

    agent {
        node any {
        }
    }

    environment {
        GIT_URL : 'https://github.com/jayavardhan123/simple-java-maven-app.git'
    }

    stages {

        stage ("SourceCheckout") {
            steps {
                git credentialsId: 'github_credentials',
                    url: environment.GIT_URL
            }
        }
    }
}