pipeline {
    agent any
    stages {
        stage("Test") {
            when {
                environment(name: "BRANCH_NAME", value: "dependabot/maven/mysql-mysql-connector-java-8.0.28")
            }
            steps {
                echo "Hello World!"
            }
        }
    }
}
