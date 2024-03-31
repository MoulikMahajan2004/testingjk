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
                emailtext subject:"buildingpipeling",
                          boy:"hi",
                           to: 'moulik4815.be22@chitkara.edu.in',
                          attachLog: true
            }

            failure
            {
                emailtext subject:"build droped",
                          boy:"hi test failes",
                           to: 'moulik4815.be22@chitkara.edu.in',
                          attachLog: true
            }
        }

}
