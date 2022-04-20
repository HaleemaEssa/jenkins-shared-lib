@Library("shared-library") _
pipeline {
    agent any
    stages {
        stage('Con1') {
            steps {
                //helloWorldExternal(dayOfWeek:"Thursday",name:"Haleema")
                dockerBuild.git-branch(main,https://github.com/HaleemaEssa/temp-test.git)
                dockerBuild.login()
                dockerBuild.build('haleema/test-temp:latest')
                dockerBuild.push('haleema/test-temp')
            }
        }
    }
}
