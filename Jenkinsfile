pipeline {
    agent {
        any {
            image 'maven:3-alpine' 
            args '-v /home/djp/.m2:/root/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
