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
sh ' git clone https://github.com/chethanmahesh03/excel-webapp-streamlit.git -b master'
}
}
stage ('deploy') {
    steps {
        sh ' mv /var/lib/jenkins/workspace/mvn_web/awsweb/*  /var/www/html'
        
    }
}
}
}
