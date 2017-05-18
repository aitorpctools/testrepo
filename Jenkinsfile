pipeline {
   agent any

   stages {
      
      def fileData
      stage('Preparation') {
         git 'https://github.com/aitorpctools/testrepo.git'
      }
      stage('ReadFile') {
          fileData = readFile 'README.md'
      }
      stage('Print') {
          println fileData
      }
   }
}
