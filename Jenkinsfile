pipeline{
agent "any"
 tools{
      jdk "jdk8"
      maven  "maven2"
}
stages{
    stage("gitcode"){
        steps{
         git branch: 'main', url: 'https://github.com/effiong20/my-cicd-repo.git'
        }

    }
    stage("build-1"){
        steps{
         sh "mvn test"
        }
      }
    stage('SonarQube analysis') {
    environment {
        scannerHome = tool 'myscanner' // the name you have given the Sonar Scanner (Global Tool Configuration)
    }
    steps {
        withSonarQubeEnv(installationName: 'sonar') {
            sh 'mvn sonar:sonar'
        }
    }

   }
 }
}