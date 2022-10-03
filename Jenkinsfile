node {
    stage("SCM") {
        git 'https://github.com/sirish12389/java-tomcat-maven-example.git'
    }
    stage("Maven") {
        sh 'mvn package'
    }
    stage("Archive") {
        archiveArtifacts artifacts: 'target\\java-tomcat-maven-example.war', followSymlinks: false
    }
}