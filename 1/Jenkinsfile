pipeline{
    agent{
        docker{
            image 'jenkinsslacedotnet'
        }
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
                archiveArtifacts artifacts: 'src/EAApp/bin/Debug/netcoreapp3.1/publish/*'
            }
        }
    }

}