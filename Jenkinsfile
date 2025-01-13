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
