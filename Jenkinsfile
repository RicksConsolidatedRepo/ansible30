pipeline {
agent {
 label "master"
}
stages {
    
    stage('Deploy the application'){
    steps{
        ansiblePlaybook installation: 'ansible', inventory: 'project1/dev', playbook: 'project1/deployweb.yml', vaultCredentialsId: 'ansible_vault'
    }
}
}
}
