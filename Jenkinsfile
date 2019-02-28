node ('master'){
  stage('check-out'){
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/kunalkumar229/test.git']]])
  }
  stage('list'){
   sh 'ls'; 
    sh 'javac hello.java'
    sh 'java hello'
  }
}
