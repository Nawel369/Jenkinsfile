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
              //Stimuler le déploiement en copiant les fichiers vers un répertoire de déploiement
                script { def deployDir="C:\\Users\\lenovo\\Desktop\\pipeline"
                        //bat "mkdir ${deployDir}" 
                        bat "copy index.php ${deployDir}\\"
                        echo "Déploiement réussi dans ${deployDir}"
                    }
                    }
                    }

      post {
        always {
          echo 'This runs always'
               }
        success {
          echo 'This runs on success'
                }
        faillure {
          echo 'This runs is failure'
                }
            }
        
                }
          }

