pipeline
{
agent any	
stages

{ stage ('scm checkout')
 {  steps {git branch: 'master', url: 'https://github.com/debajrouth/maven-project'}         //use pipeline syntax generator to generate script

 }

{stage ('code compile')
 {steps { withMaven(globalMavenSettingsConfig: 'null', jdk: 'JDK_HOME', maven: 'MAVEN_HOME', mavenSettingsConfig: 'null')  
         { sh 'mvn compile'}
}

}
}	
