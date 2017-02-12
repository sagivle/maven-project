node {
    
stage('repo') {
    git credentialsId: '7a9fb8f9-dc96-4c39-a046-5219a056916c', url: 'https://github.com/sagivle/maven-project.git'
}
  def mvnTool = tool 'local-maven'  
   
stage("build app") {
    sh "${mvnTool}/bin/mvn clean install"  
  }
}

