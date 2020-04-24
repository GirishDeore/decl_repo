pipeline {
   agent any

   stages {
      stage('checkout') {
         steps {
            checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '4befa143-6814-42b9-bb25-86ec50fe1492', url: 'https://github.com/GirishDeore/decl_repo.git']]])
         }
      }
       stage('archiev artifact') {
         steps {
            echo 'data is archieved'
         }
      }
       stage('git') {
         steps {
            git credentialsId: '4befa143-6814-42b9-bb25-86ec50fe1492', url: 'https://github.com/GirishDeore/decl_repo.git'
         }
      }
   }
}
