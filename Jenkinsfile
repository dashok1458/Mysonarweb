pipeline {
agent any 
stages{
stage("checking code"){
steps{
checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'b9954eff-72d9-4d0d-9caf-d98c4bdb5b39', url: 'https://github.com/dashok1458/Mysonarweb.git']]])
}
}
stage("mvn clean"){
steps{
bat "mvn clean install"

}
}
}
}
