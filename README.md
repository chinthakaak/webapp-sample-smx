# webapp-sample-smx
## This shows how to deploy normal webapp war on servicemix 5.5. this uses tomcat sample.

1. For Service mix 5.5 war deployment.
install -s webbundle:http://tomcat.apache.org/tomcat-5.5-doc/appdev/sample/sample.war?Bundle-SymbolicName=tomcat-sample&Web-ContextPath=/sample

2. For smx 4.x deployment
Web-ContextPath=/sample has changed to Webapp-Context=/sample
install -s webbundle:http://tomcat.apache.org/tomcat-5.5-doc/appdev/sample/sample.war?Bundle-SymbolicName=tomcat-sample&Webapp-Context=/sample

# Deployment Steps
1. Install ServiceMix 5.5.0
Download: https://servicemix.apache.org/downloads/servicemix-5.5.0.html

2. karaf@root> install -s webbundle:http://tomcat.apache.org/tomcat-5.5-doc/appdev/sample/sample.war?Bundle-SymbolicName=tomcat-sample&Web-ContextPath=/sample

3. In browser, go to http://localhost:8181/sample/index.html
