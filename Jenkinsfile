@Library("shared-library") _
pipeline {
    environment {
        DOCKERHUB_CREDENTIALS=credentials('haleema-dockerhub')
    }
    agent any
    stages {
        stage('Con1') {
            steps {
                //helloWorldExternal(dayOfWeek:"Thursday",name:"Haleema")
                gitbranch("'main', url: 'https://github.com/HaleemaEssa/temp-test.git'")
                //git branch: 'main', url: 'https://github.com/HaleemaEssa/temp-test.git'
                login()
                dockerBuild("haleema/test-temp:latest")
                push("haleema/test-temp")
            }
        }
    }
}
