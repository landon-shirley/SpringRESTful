pipeline{

  agent any
  tools {maven "Mavenv3"}

  stages{

    stage("checkout"){

      steps{

        git branch: "main" , url: "https://github.com/landon-shirley/SpringRESTful.git"
      }
    }

    stage("build"){

      steps{

        sh "mvn compile"
      }
    }

    stage("test"){

      steps{

        sh "mvn test"
      }
    }
}
}
