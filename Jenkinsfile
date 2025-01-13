pipeline {
	agent any
	stages {
		stage ('Checkout') {
			steps {
				echo "test"
				checkout scm	
			}
		}
		stage ('Build') {
			steps {
				echo "Build"
				bat "cd C:\test\EasyDevOps-ITM-550937"
				bat "git pull"
				bat "dotnet Build \"${workspace}\\ConsoleApp\\ConsoleApp.csproj\" -c Release -o out"
			}
		}	
		stage ('Test') {
			steps {
				echo "Test"
				
			}
		}
	}
}
