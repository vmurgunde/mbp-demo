pipeline{
  agent any
  stages{
    stage("Maven Build"){
      when{
        branch 'develop'
      }
      steps{
        echo "maven build......"
      }
    }
    stage("Sonar Analysis"){
      when{
        branch 'develop'
      }
      steps{
        echo "Sonar analysis....."
      }
    }
   stage("Deploy To Dev"){
      when{
        branch 'develop'
      }
      steps{
        echo "deploying to development....."
      }
    }
   stage("Deploy To QA"){
      when{
        branch 'test'
      }
      steps{
        echo "deploying to QA....."
      }
    }
    stage("Deploy To Prod"){
      when{
        branch 'main'
      }
      steps{
        echo "deploying to Prod....."
      }
    }
  }
}
