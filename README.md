# Maven

How to install Java

  1) sudo apt-get update -y
  2) sudo apt-get upgrade -y
  3) sudo apt-get update
  4) sudo apt-get install default-jre
  5) sudo apt-get install default-jdk
  6) sudo add-apt-repository ppa:webupd8team/java
  7) sudo apt-get update
  8) sudo update-alternatives --config java
  

how to add JDK to Global Tool Configuration

  1) cd /usr/lib/jvm/
  2) ls and cd to version you like
  3) pwd to find home of JDK

maven installation on apt
  
  1) sudo apt update
  2) sudo apt install maven
  3) mvn -version
   
maven installation with apache enverment
  1) cd /tmp/
  2) sudo wget https://downloads.apache.org/maven/maven-3/3.6.3/binaries/apache-maven-3.6.3-bin.tar.gz
  3) sudo cp -r file to /opt/
              or
     sudo tar xf /tmp/apache-maven-*.tar.gz -C /opt         
  4) sudo tar xf /tmp/apache-maven-3.6.3.tar.gz 
  5) sudo mv apache-maven-3.6.3/ apache-maven
  6) sudo nano /etc/profile.d/maven.sh
            export JAVA_HOME=/usr/lib/jvm/default-java
            export M2_HOME=/opt/maven
            export MAVEN_HOME=/opt/maven
            export PATH=${M2_HOME}/bin:${PATH}
  7) sudo chmod +x /etc/profile.d/maven.sh
  8) source /etc/profile.d/maven.sh
  9) mvn -version

   
                             

  
