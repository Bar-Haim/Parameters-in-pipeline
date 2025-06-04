pipeline {
    agent any

    parameters {
        string(name: 'USERNAME', defaultValue: 'bar', description: 'הכנס שם משתמש')
        choice(name: 'ENV', choices: ['dev', 'staging', 'prod'], description: 'בחר סביבה להרצה')
    }

    stages {
        stage('Print Parameters') {
            steps {
                echo "👤 שלום ${params.USERNAME}!"
                echo "🌍 בחרת להריץ על סביבה: ${params.ENV}"
            }
        }
    }
}
