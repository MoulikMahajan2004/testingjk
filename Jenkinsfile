pipeline{
    agent any
        stages
        {
           stage('Build') {
            steps {
                echo 'building my code using the npm for react'
                echo'npm install'
                echo'npm run build'
            }
        }
        
        stage('Unit and Integration Tests') {
            steps {
                echo 'Running unit test and integration'
            }
        }
        }
        post
        {
            success
            {
                emailext subject:"buildingpipeling",
                          body:"hi",
                           to: 'moulik4815.be22@chitkara.edu.in',
                          attachLog: true
            }

            failure
            {
                emailext subject:"build droped",
                          body:"hi test failes",
                           to: 'moulik4815.be22@chitkara.edu.in',
                          attachLog: true
            }
        }

}
