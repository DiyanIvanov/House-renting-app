pipeline{
    agent any

    stage("Restore Dependancies"){
        steps{
            bat 'dotnet restore'
        }
    }
    stage("Build App"){
        steps{
            bat 'dotnet build --no-restore'
        }
    }
    Stage("Test App"){
        bat 'dotnet test --no-build --verbosity normal'
    }
}