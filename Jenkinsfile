pipeline { 
    agent any
    tools { 
        maven 'Maven 3.5.4' 
        jdk 'jdk8' 
    } 
    stages {
    	stage ('Initialize') {
            steps {
                sh '''
                	echo "M2_HOME = ${M2_HOME}"
                    echo "PATH = ${PATH}"
                ''' 
            }
        }
        stage('Build') { 
            steps { 
               echo 'This is a minimal pipeline.'
               sh "mvn clean install"
            }
        }
    }
}