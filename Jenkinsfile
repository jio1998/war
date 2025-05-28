pipeline{
agent any
  tools{
    maven "maven-3.9.9"
  }
stages{
stage("code")
{
steps{
git branch: 'dev', credentialsId: '7143caf5-851c-4b07-9282-c3c6fea53410', url: 'https://github.com/jio1998/war.git'
}
}
  stage("Build"){
    steps{
      sh "mvn clean package"
    }
  }
}
}
