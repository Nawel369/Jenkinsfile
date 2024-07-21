pipeline {
agent any
  stages {
         stage ('checkout') {
                  steps  {
                          git branch: "main", url: "https://github.com/Nawel369/pipeline.git"
                       }
      
                     }
            stage ('Build') {
                   steps {
                 bat "php index.php"
                         }
                           }    
       stage ('Test') {
                 steps {
                 echo "Test Phase"
                      }
                      }
       stage ('Deploy') {
                steps {
                echo "Build Phase"
                      }
                       }
                }
          }

