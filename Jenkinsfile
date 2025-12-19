pipeline {
    agent { label 'ansiblejenkins' }
    stages {
        stage("Execute Ansibleplaybook") {
            steps {
             ansiblePlaybook credentialsId: '100c7b37-efe8-4766-a91b-3690463e12b5', disableHostKeyChecking: true, installation: 'Ansible', inventory: '/etc/ansible/hosts', playbook: '/etc/ansible/roles/tomcat_deploy.yml', vaultTmpPath: ''   
            }
        }
    }
}
