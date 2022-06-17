pipeline {
    agent any
    stages{
        stage('scm-git'){
            steps{
                git :: 'https://github.com/jayanth197/testcase_cintap.git'
            }
         }
         stage('Build'){
             steps{
                 'mvn clean install package'
             }
         }
         stage('Testing'){
             steps{
                 junit '/test.xml'
             }
         }
    }
}
