@Library("shared-library") _
pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                helloWorldExternal(dayOfWeek:"Thursday",name:"Haleema")
            }
        }
    }
}
