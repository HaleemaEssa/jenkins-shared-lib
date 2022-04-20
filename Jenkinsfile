@Library("shared-library") _
pipeline {
    agent any
    stages {
        stage('Con1') {
            steps {
                //helloWorldExternal(dayOfWeek:"Thursday",name:"Haleema")
                gitbranch('main','https://github.com/HaleemaEssa/temp-test.git')
                login()
                build('haleema/test-temp:latest')
                push('haleema/test-temp')
            }
        }
    }
}
