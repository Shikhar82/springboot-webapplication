# Deploy web application in Elastic Bean Stack

# Pre-Requisites
    Springboot Application
    Install Maven
# Clone code using below command
    git clone https://github.com/Naresh240/springboot-webapplication.git
    cd springboot-webapplication
# Build Artifact
    mvn clean install
# Deploy springboot application with Tomcat
  Tomcat Setup:
    
    cd /opt
    wget https://downloads.apache.org/tomcat/tomcat-9/v9.0.46/bin/apache-tomcat-9.0.46.tar.gz
    cd apache-tomcat-9.0.46 tomcat
  
  Start tomcat:
    
    cd /opt/tomcat/bin
    ./startup.sh
  
  Copy springboot artifact to Webapps Directory:
    
    cd springboot-webapplication
    cp target/mavewebappdemo-2.0.0-SNAPSHOT.war /opt/tomcat/webapps/mavewebappdemo.war

# Check output of application
  ![image](https://user-images.githubusercontent.com/58024415/120204004-f5f5f100-c245-11eb-8c4b-4c1128434d8e.png)
