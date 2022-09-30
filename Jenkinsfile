node('jdk8') {
    stage('VCS') {
        git branch:'teja', url: 'https://github.com/tejachennuru1/spring-framework-petclinic.git'
    stage("build") {
        sh '/usr/bin/mvn /usr/share/man/man1/mvn.1.gz'
    }  
    stage("archive results") {
        junit '**/surefire-reports/*.xml'
    }      
        }
}   