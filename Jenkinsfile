node {
  stage("Clone the project") {
    git branch: 'master', url: 'https://github.com/archie252000/JavaDevopsAssignment'
  }

  stage("Compilation") {
  bat "mvn https://github.com/archie252000/JavaDevopsAssignment/pom.xml compile"
  }

  stage("Tests and Deployment") {
    stage("Runing unit tests") {
      sh "./mvnw test -Punit"
    }
    
  }
}