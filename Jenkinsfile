pipeline{
  agent any
  stages{
    stage("new stage"){
      step("Hello"){
       sh "echo hello world" 
      }
      stage("hello"){
        step("new hello"){
         sh "echo bye-bye" 
        }
      }
    }
  }
}
