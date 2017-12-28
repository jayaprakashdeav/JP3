pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        bat 'echo Hello'
      }
    }
    stage('Restore Nuget') {
      steps {
        bat 'C:\\JP\\Nuget\\nuget.exe restore "C:\\Users\\jayaprakash.s\\Documents\\Visual Studio 2017\\Projects\\Hello_World\\Hello_World.sln"'
      }
    }
    stage('Build using Ms build') {
      steps {
        bat '"msbuild.exe" "C:\\Users\\jayaprakash.s\\Documents\\Visual Studio 2017\\Projects\\Hello_World\\Hello_World.sln"'
      }
    }
  }
}