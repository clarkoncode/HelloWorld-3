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
                    powershell ("""
                        \$fileName = [DateTime]::Now.ToString("yyyyMMdd-HHmmss") + ".zip";
                        New-Item -Path "C:\\Temp\\$fileName";
                    """)
                }
            }
        }
    }
}
