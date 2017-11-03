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

stage ('TEST') {
    echo 'TEST'
}

stage ('DEPLOY') {
    echo 'DEPLOY'
}
}
