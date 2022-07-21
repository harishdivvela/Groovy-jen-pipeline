pipeline {
    agent any
    stages {
        stage("Test") {
            when {
                environment(name: "BRANCH_NAME", value: "master")
            }
            steps {
                echo "Hello World!"
            }
        }
    }
}
