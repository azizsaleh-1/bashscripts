node(){
    stage('Checkout'){
        checkout scm
    }
    stage('Printing Parameter'){
        sh "echo ${environment}"
    }
    stage('Build'){
        sh "sh untilloop.sh"
    }
    stage('Array'){
        sh "sh array"
    }
    stage('Notify'){
        sh 'mail -s "the job ran fine" lokesh.mydilse@gmail.com'
    }
}