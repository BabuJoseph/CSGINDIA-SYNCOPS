node{
    stage('SCM Checkout'){
    
    git credentialsId: 'git-creds', url: 'https://github.com/BabuJoseph/CSGINDIA-SYNCOPS.git'
    
   }
   stage('Mvn Package'){
     sh 'mvn clean package'   
       
   }
   stage('Build Docker Image'){
       sh 'docker build -t babujoseph5757/my-app:2.0.0 .'
   }
   
}
