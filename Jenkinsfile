pipeline
{
    stages
    {
        stage('Get Source')
        {
            steps
            {
                script
                {
                    powershell "New-Item -Path "C:\Temp\HelloWorld3-$([DateTime]::Now.ToString("yyyyMMdd-HHmmss") + ".zip")""
                }
            }
        }
    }
}
