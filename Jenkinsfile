pipeline {
    agent any
    stages {

        stage('apache update welcome.html'){
          steps{
		    echo 'copy welcome.html from Jenkins through Git'
                //sh 'mkdir from-jenkins'
                //sh 'touch from-jenkins/test.txt'
		    echo 'running palybook' 
                sh '''
                   ansible-playbook apache-html.yml -l qa -i inventory; 
                '''
                }
        }

}
}
