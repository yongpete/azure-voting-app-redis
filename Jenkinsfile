node {
  parameters {
    string(name: 'ENVIRONMENT', defaultValue: 'prod')
  }
  stage('PowerShell') {
    switch("${params.ENVIRONMENT}") { 
      case 'qa': 
        println "This is a test"
        pwsh(script: "New-Item -Path $WORKSPACE -ItemType File -WhatIf")
      case 'prod': 
        println "This is not a test"
        pwsh(script: "New-Item -Path $WORKSPACE -ItemType File")
    }
  } 
}