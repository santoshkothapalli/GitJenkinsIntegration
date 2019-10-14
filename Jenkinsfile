node {
    stage('Version Check'){
           echo("---starting jenkins build process");
    bat 'node --version' 
    checkout([$class: 'GitSCM', branches: [[name: '*/master']],userRemoteConfigs: [[url: 'https://github.com/santoshkothapalli/GitJenkinsIntegration.git']]])
    bat "mvn clean verify"
    }
    
    echo("--checkout successful")

}
