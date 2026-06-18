pipeline{
  agent any
  tools{
    maven 'Maven'
  }
  stages{
    stage('Checkout'){
      steps{
        git 'https://github.com/Ranjana2225/selenium1.git'
      }
    }
    stage('Build'){
      steps{
        sh 'mvn clean install'
      }
    }
    stage('Run application'){
      steps{
        sh 'mvn exec:java -Dexec.mainClass="com.example.App"'
      }
    }
  }
}
