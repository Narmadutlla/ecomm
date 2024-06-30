
pipeline {
   agent any


   stages {
       stage('LMS Code Analysis') {
           steps {
               echo 'Preparing Sonar Analysis'
               sh ' index.html && sudo docker run --rm -e SONAR_HOST_URL="http://3.96.206.45:9000" -v ".:/usr/src" -e SONAR_TOKEN="sqp_f563a5a5559e418d23de9c352714f2308391ca99" sonarsource/sonar-scanner-cli -Dsonar.projectKey=ecomm'
               echo 'Completed Sonar Analysis'
           }
       }
   }
}
