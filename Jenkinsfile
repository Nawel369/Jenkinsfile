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
                   echo "Build Phase"
                         }
                           }    
       stage ('Test') {
                 steps {
                 echo "Test Phase"
                      }
                      }
    
                }
          }

