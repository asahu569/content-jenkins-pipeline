pipeline {
	agent any

	stages {
		stage('build') {
			steps {
			sh 'javac -d .src/*.java'
			sh 'echo Main-Class: Rectangulator > Manifest.MF'
			sh 'jar -cvmf MANIFEST.MF rectangle.jar *.class'
				}
			}
		}
	}
