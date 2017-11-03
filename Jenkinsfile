node ('master') {
stage ('SCM') {
    git 'https://github.com/carreerit/mavenrepo.git'
}

stage ('BUILD') {
    sh 'mvn clean compile package'
}

stage ('UPLOAD') {
    sh 'mvn deploy'
}
    
stage ('APPROVE') {
   input 'Do you want to do the deployment'
}

stage ('TEST') {
    echo 'TEST'
}

stage ('DEPLOY') {
    echo 'DEPLOY'
}
}
