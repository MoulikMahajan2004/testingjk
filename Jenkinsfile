pipeline{
    agent any
        stages
        {
            stage('build')
            {
                steps
                {
                    echo'building jenkins'
            
                }
            }
            stage('Testing')
            {
                steps
                {
                    echo'Test jenkins'
            
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
