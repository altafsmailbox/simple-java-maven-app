node{ 
  environment {
    PATH = "C:\\Program Files\\Git\\usr\\bin;C:\\Program Files\\Git\\bin;${env.PATH}"
  stage('SCM Checkout'){
    git 'https://github.com/altafsmailbox/simple-java-maven-app/'
  }
  stage('Compile package'){
    def mvnHome = tool name: 'maven', type: 'maven'
    sh "${mvnHome}/bin/mvn -B -DskipTests clean package"
  }
}
}
