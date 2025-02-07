import hudson.model.*;
pipeline 
{
    agent any 
    stages 
    {
        stage('Build') 
        { 
            steps 
            {
                script
                {
                    json_path = "${env.WORKSPACE}/channel_config_1002.json"
                    content = readFile json_path
                    echo(content)
                    echo("1over")
                }
                echo("Build")
            }
        }
        stage('测试') 
        { 
            steps 
            {
                script
                {
                    sh 'java -version'
                }
                echo("Test")
            }
        }
        stage('Deploy') 
        { 
            steps 
            {
                script
                {
                    timeout(1)
                    {
                        sh('java -version')
                        //sleep(31)
                    }
                }
                echo("Deploy")
            }
        }
    }
}
