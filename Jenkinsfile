pipeline {
    agent any
        stage('build') {
               withMaven(
        		maven: 'M3',
        		mavenSettingsConfig: 'apache-maven-3') {
      					sh "mvn clean install"
			}
		}
}