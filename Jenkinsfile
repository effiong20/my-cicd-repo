pipeline{
agent "any"
 tools{
      jdk "jdk11"
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
         sh "mvn compile test"
        }

    }
}
    }
 