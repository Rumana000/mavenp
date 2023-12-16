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
}    

  
