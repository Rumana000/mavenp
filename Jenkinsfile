@Library("mylibrary")_
node('built-in')
{
    stage('cont down')
    {
      cicd.newGit('https://github.com/Rumana000/maven45.git')

    }
    stage('cont build')
    {
      cicd.newMaven()

    }
    stage('cont deploy')
    {
        cicd.newDeploy("${env.WORK_SPACE}","172.31.47.3","testapp")
    }
    stage('cont test')
    {
         cicd.newGit('https://github.com/intelliqittrainings/FunctionalTesting.git')
         cicd.newrunSelenium("${env.WORK_SPACE}")
    }
    stage('cont delivery')
    {
        cicd.newDeploy("${env.WORK_SPACE}","172.31.42.203","prodapp")
    }
}
 
