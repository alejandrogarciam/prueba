pipeline {
	agent any
	stages{
		stage('Primera inicializacion'){
			steps{
				sh 'echo inicializando...'
			}
		}
		stage('checando docker'){
			steps{
				sh 'sudo docker ps'
			}
		}
		stage('construir imagen'){
			steps{
				sh 'sudo docker build --tag=php54local .'
				sh 'sudo docker images|grep php54local'
			}
		}
	}
}
