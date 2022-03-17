node{
    def gradleHome = tool name: "gradle7.3.2"
    stage("check out SCM"){
        git credentialsId: 'github_crede1', url: 'https://github.com/pravschevuru/sonartest.git'
    }
    
    stage("sonarqube code analysis"){
        sh "ls -lrth"
        //sh "${gradleHome}/bin/gradle sonarqube"
        sh "gradlew sonarqube"
        
    }
}
