pipeline {
agent any
stages {
stage('clean workspace') {
steps {
sh 'rm -r *'
sh 'rm -r ../../../../www/html/*'
}
}
stage ('clonning') {
steps {
sh ' git clone https://gitlab.com/chethanmahesh03/awsweb.git -b master'
}
}
stage ('deploy') {
    steps {
        sh ' mv /var/lib/jenkins/workspace/mvn_web/awsweb/*  /var/www/html'
        
    }
}
}
}
