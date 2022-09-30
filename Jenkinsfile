node('jdk8') {
    stage('VCS') {
        git branch:'REL_INT_1.0', url: 'https://github.com/GitPracticeRepo/spring-petclinic.git'
    }
    stage("build") {
        sh '/usr/bin/mvn /usr/share/man/man1/mvn.1.gz'
    }  
    stage("archive results") {
        junit '**/surefire-reports/*.xml'
    }      
        }
    