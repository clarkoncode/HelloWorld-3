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
                    powershell ("""
                        \$name = \"Nate\"
                        Write-Host \"Hello World\"
                        Write-Host \$name
                    """)
                    powershell ("""
                        \$fileName = [DateTime]::Now.ToString("yyyyMMdd-HHmmss") + ".zip";
                        New-Item -Path "C:\\Temp\\$fileName";
                    """)
                }
            }
        }
    }
}
