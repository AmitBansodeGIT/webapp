pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                mvn install
            }
        }
        stage("deploy") {
          step {
            cp target/WebApp.war /mnt//mnt/apache-tomcat-9.0.69/webapps/
          }
        }
    }

}
