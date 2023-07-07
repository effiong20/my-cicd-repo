pipeline{
agent "any"
 tools{
      jdd "jdk11"
      maven  "maven2"
}
stages{
    stage("gitcode"){
        step{
         git branch: 'main', url: 'https://github.com/effiong20/my-cicd-repo.git'
        }

    }
}
    }
 