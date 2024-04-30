pipeline
{
    agent any
    stages
    {
        stage('Initialize')
        {
            steps
            {
                script
                { 
                    echo 'Starting the Pipeline'  
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