pipeline {
agent {
label 'newnodes'
}

stages {

stage ('Checkout') 
{
steps
    {
    
        checkout scm
        
    }
    
}
stage ('Creation of the folder ') 
{
    steps
    {
       sh "cd /home/ubuntu ; sudo mkdir trstfolder " 
    }
}

   
stage ('Creatin the folder on differen server ')
    {
    steps {
        node (' Ansible-server'){

        sh "cd /var/www; sudo mkdir devopsjenkins"    
        }
}

    }   
    

}
    
    
}
