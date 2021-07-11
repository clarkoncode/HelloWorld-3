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
                    powershell ("\$name = \"Nate\"")
                    powershell ("Write-Host \"Hello World\"")
                    powershell ("Write-Host $name")
                    powershell ("""
                        \$fileName = [DateTime]::Now.ToString("yyyyMMdd-HHmmss") + ".zip";
                        New-Item -Path "C:\\Temp\\$fileName";
                    """)
                }
            }
        }
    }
}
