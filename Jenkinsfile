pipeline{
	agent any
	tools{
		gradle 'Gradle'
		jdk 'JDK
	}
	stages{
		stage('Checkout'){
			steps{
				git branch:'main',url:'https://github.com/LikithReddy0409/Exam4.git'
			}
		}

		stage('Build'){
			steps{
				sh 'gradle run'
			}
		}

		stage('Run Application'){
			steps{
				sh 'gradle display'
			}
		}
	}
		post{
			success{
				echo 'Build Successfull'
			}
			Failure{
				echo 'Build Failed'
			}
		}
	}

		
			
			
