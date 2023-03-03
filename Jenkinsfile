pipeline {
    agent {
        label "linux"
    }
    stages {
        stage('Checkout repo'){
            steps {
                git credentialsId: 'da5cf165-10a6-4a61-a089-d04b6a045510', url: 'git@github.com:ana17519/my_own_collection.git'
            }
        }
        stage ('Prepare for molecule'){
            steps {
                sh 'pip3 install --force "molecule==3.5.2" "molecule_docker==0.3.3" yamllint ansible-lint'
            }
        }
        stage('Run Molecule'){
            steps {
                sh 'cd my_own_namespace/yandex_cloud_elk/roles/my-collection/tests'
                sh 'molecule init scenario'
                sh 'molecule test'
            }
        }
    }
}