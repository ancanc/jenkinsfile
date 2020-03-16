node ('C'){
    stage ('GIT'){
        git 'https://github.com/spring-projects/spring-petclinic.git'
    }
    stage ('MVN'){
        sh 'mvn clean'
    }
    stage ('mail'){
	mail body: 'Success', subject: 'Build State', to: 'nagarjunamukku@gmail.com'
    }
}
