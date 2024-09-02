pipeline {
	agent{
	label 'label-2'
	}
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh 'JAVA_HOME=/home/shiro/demoslavedir/jdk-11.0.24 /home/shiro/demoslavedir/apache-maven-3.9.8/bin/mvn install'
	                 }}
		stage('Deployment'){
		    steps {
			sh 'cp target/Project9.war /home/shiro/demoslavedir/apache-tomcat-9.0.93/webapps'
			}}	
}}
