pipeline {
	agent any 
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/virat/appfile/apache-maven-3.9.0/bin/mvn install'
	                 }}
		stage('Deployment'){
		   steps {
		sh 'cp target/slave1.war  /home/avinash/Downloads/tar2-file/apache-tomcat-9.0.85/webapps'
			}}	
}}
