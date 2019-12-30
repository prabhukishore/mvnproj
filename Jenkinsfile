node{
  stage('scm-checkout'){
    git ""
  }
  stage('compile-package'){
    def mvnhome= tool name: 'maven-3.6.3', type: 'maven'
    sh "$(mvnhome)/bin/mvn package"
  }
}
