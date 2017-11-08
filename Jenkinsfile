pipeline {
    agent { 
        node {
            label 'shared' 
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
