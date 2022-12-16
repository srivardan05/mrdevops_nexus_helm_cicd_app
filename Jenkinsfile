Pipeline{
 Agent any 
Stages{
stage(‘sonar quality status’){
 Agent{
 Docker{
  Image ‘maven’
}
}
}
}
}
Steps{
 Script{
WithsonarqubeEnv(credentialsId: ‘soar-token’) {
Sh ‘man clean package sonar:sonar’
}
}
}
