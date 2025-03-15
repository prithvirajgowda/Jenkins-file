pipeline {
agent any 
stages {
      stage ('build') {
                 steps {
                    echo " this is build stage"
                   }
                  }
     stage ('deploy') {
               steps {
                  echo " this is deploy stage"
               }
               }   
     stage ('test') {
        parallel{
         stage ('test1') {
            steps {
            echo "this is test1"
            }
         }
      stage ('test2') {
      steps {
echo "this is test2"
      }
      }
        }
     }
}
}
