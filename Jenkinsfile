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
                 bat "php test.php"
                      }
                      }

         stage ('Deploy') {
              steps {
              echo "Build Phase"
                    }
                    }
                }
          }

