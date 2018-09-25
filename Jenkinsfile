pipeline {
  agent {
    node {
      label 'Test'
    }

  }
  stages {
    stage('Job') {
      parallel {
        stage('Job') {
          steps {
            build 'Belgium CreditCardFR'
          }
        }
        stage('') {
          steps {
            build 'Belgium CreditCardNL'
            build 'Belgium PersLoanNL'
          }
        }
      }
    }
  }
}