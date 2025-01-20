pipeline {
agent any
stages {
stage('Checkout') {
steps {
git url:
'https://github.com/Kirankale11/AnsibleJenkinsPipeline.git',
credentialsId: 'github-credentials-id'
}
}
stage('Run Ansible Playbook') {
steps {
ansiblePlaybook playbook:
'NGINX_INSTALL_playbook.yml', inventory: 'inventory.ini',
credentialsId: 'github-credentials-id	'
}
}
}
}
