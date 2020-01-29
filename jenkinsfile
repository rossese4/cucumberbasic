 node('master') {
    stage('Git Checkout') {
        git 'https://github.com/executeautomation/cucumberbasic.git'
    }
    
    stage('Compile') {
        bat label: '', script: 'mvn compile'
    }
    
    stage('Approve deploy to CERTIFICA') {
        input '¿Preparados para desplegar en CERTIFICA?'
    } 
 
}
