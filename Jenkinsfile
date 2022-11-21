pipeline {       
        agent any 
        stages {
        node('Built-In Node'){        
        stage("Build") {               
                steps {                  
                        sh "mvn --version"                 
                }        
                }
                }  
        node('slave_node1'){   
        stage("Compile") {             
                steps {                  
                        sh "mvn compile"            
                }        
                }
                }
        node('slave_node2'){
        stage("Unit Test") {             
                steps {                  
                        sh "mvn test"            
                }        
                } 
                }             
        }
}


