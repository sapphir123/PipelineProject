import hudson.model.*;

node("测试节点") {
    stage('Build') 
    { 
        json_path = "${env.WORKSPACE}/channel_config_1002.json"
        content = readFile json_path
        echo(content)
        echo("over")
        echo("Build")
    }
    stage('Test1') 
    { 
        sh 'echo "Hello, World!"'
        echo("Test")
    }
    stage('Deploy') 
    { 
        echo("Deploy")
    }
}
