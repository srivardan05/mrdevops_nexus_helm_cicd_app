Pipeline{
 agent any 
Stages{
stage(‘sonar quality status’){
 agent{
 Docker{
  Image ‘maven’
}
}
}
}
}
Steps{
 script{
 withSonarQubeEnv(credentialsId: 'e23ed37a-e7b8-402f-a285-93d0388daf6a') 
     }
Sh ‘man clean package sonar:sonar’
}
}
}
