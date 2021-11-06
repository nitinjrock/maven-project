pipeline
{
    agent any 
    stages 
    { 
    stage ('SCM checkout')
    { steps { git branch: 'master', url: 'https://github.com/nitinjrock/maven-project.git' } }
        
        stage ('Build the code')
        {steps { withMaven(jdk: 'local_jdk', maven: 'local_maven _3.3.9') {
           sh 'mvn clean package'                // need to provide maven actual command
} }}
        
    }
    
}
