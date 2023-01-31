pipeline {
    agent { lable 'Ansible'}
    stages {
        stage ('git') {
            steps {
                git branch: 'main', url: 'git@github.com:krishna5683akp/ContiniousIntigrationAnsible.git'
            }
        }
        stage ('ansivle') {
            steps {
                sh 'ansible-playbook -i hosts java.yaml'
            }
        }
    }
}