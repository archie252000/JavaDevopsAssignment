node {
  stage("Clone the project") {
    git branch: 'main', url: 'https://github.com/archie252000/JavaDevopsAssignment'
  }

  stage("Compilation") {
    sh "./mvnw clean install -DskipTests"
  }

  stage("Tests and Deployment") {
    stage("Runing unit tests") {
      sh "./mvnw test -Punit"
    }
    
  }
}