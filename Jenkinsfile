pipeline{
    
    agent any 

    
    stages{
        stage('build') {
            steps{
               script {
                  //Ensure Maven in the PATH
                      bat 'mvn -v'  // Verify Maven installation
                      bat 'mvn clean install' // Run the Maven build
                }
            }
        }
       
        stage('deploy') {
            steps{
                script {
                    bat 'docker built .'
                
            }
        }
    }
}
