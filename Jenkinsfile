pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo "building..."
		sh 'mvn package'
            }
        }
        stage('Publish Build Artifacts') { 
            steps {
               echo "publishing Artifacts..."
		archiveArtifacts 'project/target/*.war'
            }
        }
        stage('Test') { 
            steps {
               echo "Testing..."
		
            }
        }
        stage('Deploy') { 
            steps {
                echo "Deplying..." 
            }
        }
    }
}
