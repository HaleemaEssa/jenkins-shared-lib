@Library("shared-library") _
pipeline {
    agent any
    stages {
        stage('Con1') {
            steps {
                //helloWorldExternal(dayOfWeek:"Thursday",name:"Haleema")
                dockerBuild.login()
                dockerBuild.build(haleema/test-temp:latest)
                dockerBuild.push(haleema/test-temp)
            }
        }
    }
}
