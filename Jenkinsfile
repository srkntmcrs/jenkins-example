pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                // for windows slaves, use "bat" instead of "sh"
            bat 'mvn clean compile'
                //withMaven(maven : 'maven_3_5_0') {
                  //
                //}
            }
        }

        stage ('Testing Stage') {

            steps {
                 bat 'mvn test'
                //withMaven(maven : 'maven_3_5_0') {
                //
                //}
            }
        }


        stage ('Deployment Stage') {
             steps {
              bat 'mvn deploy'
                //withMaven(maven : 'maven_3_5_0') {
                  //
                //}
            }
        }
    }
}
