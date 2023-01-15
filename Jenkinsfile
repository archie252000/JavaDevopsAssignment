node {
  stage("Clone the project") {
    git branch: 'master', url: 'https://github.com/archie252000/JavaDevopsAssignment'
  }

  stage("Compilation") {
    def mvnHome = tool name: 'Maven', type: 'maven'
    bat "${mvnHome}/bin/mvn clean install"
  }

  stage("Tests and Deployment") {
    stage("Runing unit tests") {
      sh "./mvnw test -Punit"
    }
    
  }
}