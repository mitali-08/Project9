pipeline{
        agent any
        stages{
                stage(checkout){
                        steps{
                        git 'https://github.com/mitali-08/Project9.git'
                        }
                }
                stage(build){
                        steps{
                        sh 'mvn install'
                        }
                }
                stage(deploy){
                        steps{
                        cp target/Project9.war /home/mitali/Documents/devops/apache-tomcat-9.0.93/webapps
                        }
                }
                }

