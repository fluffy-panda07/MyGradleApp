pipeline{
	agent any
	tools{
		gradle 'Gradle'
		jdk 'JDK'}
	stages{
		stage('Checkout'){
			steps{ git branch:'master' ,url:'https://github.com/fluffy-panda07/MyGradleApp.git'}
			}
		stage('Build'){
			steps{
				sh 'gradle build' }
				}
		stage('Test'){
			steps{
				sh 'gradle test'}}
		stage('Run application'){
			steps{ sh 'gradle run' }}
		}
	post{
		success{ echo 'Build and deployment successfull'}
		failure{ echo 'Build failed'}
		}
		}
		
