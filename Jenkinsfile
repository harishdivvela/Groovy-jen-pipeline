pipeline {
    agent any
    stages {
        stage("Test") {
            when {
                environment(name: "BRANCH_NAME", value: "main")
            }
            steps {
                echo "Hello World!"
            }
        }
    }
}
