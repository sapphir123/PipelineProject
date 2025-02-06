pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                script{
                    json_path = "${env.WORKSPACE}/channel_config_1002.json"
                    content = readFile json_path
                    echo(content)
                    echo("over")
                }
                echo("Build")
            }
        }
        stage('测试') { 
            steps {
                script{
                    content = sh('java -version')
                    echo(content)
                }
                echo("Test")
            }
        }
        stage('Deploy') { 
            steps {
                echo("Deploy")
            }
        }
    }
}
