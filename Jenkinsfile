node('jdk8') {
    stage('VCS') {
        git branch: 'teja', url: 'https://github.com/tejachennuru1/spring-framework-petclinic.git'
    }
    stage("build") {
        sh '/usr/share/maven/bin/mvn package'
    }  
    stage("archive results") {
        junit '**/surefire-reports/*.xml'
    }      
    
     }
  