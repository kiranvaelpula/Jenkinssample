def workspace
node{
    stage("checkout")
    {
      checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/kiranvaelpula/Jenkinssample.git']]])  
      workspace=pwd()
    }
    stage("static code Analysis")
    {
        echo "static code Analysis"
    }
    stage("Test")
    {
        echo "unit test cases"
    }
    stage("Build")
    {
        echo "Build the code"
    }
    stage("Delivery")
    {
        echo "Delevering the code"
    }
}
