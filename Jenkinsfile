pipeline {
    agent any 
    stages {
        stage ('clone') {
            steps 
                {
                    git branch: 'main', url: 'https://github.com/cuonglucson/projectnet.git'
                }
        }
        stage('restore package') {
            steps
            {
                echo 'Restore package'
                bat 'dotnet restore'
            }
	    }

    }
}
