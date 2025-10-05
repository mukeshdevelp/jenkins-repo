@Library('groovy@main') _
import org.mukesh.JenkinsHello

pipeline {
    agent any

    stages {
        stage('Greet with Function') {
            steps {
                sayHello('mukesh')
            }
        }
        stage('Greet with Class') {
            steps {
                script {
                    def greeter = new JenkinsHello(this)
                    greeter.sayHelloJenkins()
                }
            }
        }
    }
}
