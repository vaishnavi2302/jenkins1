pipeline {
	 agent any 
	 
	 stages {
		stage("compile") {
			steps {
				echo "Compiling"
				bat """ javac Test1.java """
				}
			}
			
		stage ("run") {
			steps {
				echo "Running"
				bat """ java Test1"""
				}
			}
			
		stage ("docker") {
			steps {
				echo "Running Docker"
				bat """ docker run app-1 """
				}
			}
		}
	}