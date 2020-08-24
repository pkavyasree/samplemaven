node{

    stage('SCM Checkout'){
    git credentialsId: 'github-pwd', url: 'https://github.com/pkavyasree/samplemaven.git'
    }
    stage('Mvn Package'){
         def mvnHome = tool name: 'maven', type: 'maven'
         def mvnCMD = "/usr/share/maven/bin/mvn"
         sh "${mvnCMD} -f pom.xml clean package"
     } 
}
