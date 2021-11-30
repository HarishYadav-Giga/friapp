pipeline{
  agent any
  stages{
    stage("mvn build dev"){
      when {
        branch "dev"
      }
      steps{
      sh "mvn clean package"
    }
  }
 stage("uat deployment"){
      when {
        branch "uat"
      }
      steps{
      echo "uat deployment done"
    }
  }
     stage("prod deployment"){
      when {
        branch "main"
      }
      steps{
      echo "prod deployment done"
    }
  }
}
}
