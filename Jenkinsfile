pipeline
{
    agent any

    stages
    {
        stage('Get Source')
        {
            steps
            {
                script
                {
                    powershell ("Write-Host \"Hello World\"")
                    powershell ("""
                        \$fileName = [DateTime]::Now.ToString("yyyyMMdd-HHmmss") + ".zip";
                        New-Item -Path "C:\\Temp\\$fileName";
                    """)
                }
            }
        }
    }
}
