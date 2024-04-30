pipeline
{
    agent
    {
        docker
        {
            label "Python"
            image 'python:3.12.1-alpine3.19'
            args '-v /var/run/docker.sock:/var/run/docker.sock'
        }
    }
    stages
    {
        stage('Initialize')
        {
            steps
            {
                script
                { 
                    echo 'Starting the Pipeline'  
                    sh 'python --version'
                }
            }
        }
        stage('Build')
        {
            steps
            {
                script
                {
                    echo 'Building the code ...'
                }
            }
        }
    }
    post
    {
        success
        {
            script
            {
                echo 'Pipeline execution completed successfully'
            }
        }
        failure
        {
            script
            {
                echo 'Pipeline execution failed'
            }
        }
        always
        {
            script
            {
                echo 'Pipeline execution completed'
            }
        }
    }
}