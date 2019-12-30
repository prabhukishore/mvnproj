node{
  stage('scm-checkout'){
    git 'https://github.com/prabhukishore/mvnproj.git'
  }
  stage('compile-package'){
    def mvnhome= tool name: 'maven-3.6.3', type: 'maven'
    sh "${mvnhome}/bin/mvn package"
  }
}
