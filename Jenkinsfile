pipeline{
agent "any"
 tools{
      jdd "jdk11"
      maven  "maven2"
}
stages{
    stage("gitcode"){
        step{
        sh git branch: 'main', url: 'https://github.com/effiong20/my-cicd-repo.git'
        }

    }
}
    }
 