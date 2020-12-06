pipeline{    
    agent{
        docker{
            image 'jenkinsslacedotnet'
        }
    }

    parameters{
        password(name: 'PASSWORD', defaultValue: 'C@astle', description: 'jhf us fdkj')
    }
    environment{
        USER_NAME = "raja"
    }

    stages{
        stage('SCM'){
            steps {
                sh 'dotnet build "$WORKSPACE/src/EAApp/EAApp.csproj"'
            }
        }

        stage('publish'){
            steps {
                sh 'dotnet publish "$WORKSPACE/src/EAApp/EAApp.csproj"'
                echo "${env.USER_NAME}"
                echo "${params.PASSWORD}"
                archiveArtifacts artifacts: 'src/EAApp/bin/Debug/netcoreapp3.1/publish/*'

            }
        }
    }

}