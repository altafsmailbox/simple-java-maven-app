node{ 
  stage('SCM Checkout'){
    git 'https://github.com/altafsmailbox/simple-java-maven-app/'
  }
  stage('Compile package'){
    sh 'mvn package'
  }
