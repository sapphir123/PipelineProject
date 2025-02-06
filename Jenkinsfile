pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                script{
                    json_path = "${env.WORKSPACE}/channel_config_1002.json"
                    content = readFile json_path
                    echo(json_path)
                    echo("打印完毕")
                }
                echo("Build")
            }
        }
        stage('Test') { 
            steps {
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
