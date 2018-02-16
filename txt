mkdir -p src/main/java/hello
rm -r src/main/java/hello

sudo ....

tar zxvf eclipse-inst-linux64.tar.gz

jar tvf build/libs/gs-gradle-0.1.0.jar

./

查看yum库中都有那些jdk：
yum search java|grep jdk

yum -y  install java-1.8.0-openjdk
sudo yum -y install java-1.8.0-openjdk-devel

sudo yum -y remove python-javapackages.noarch

rpm -ivh jdk-7u79-linux-x64.rpm

rpm -qa|grep java

apt-cache search java|grep jdk

apt-get install openjdk-7-jdk

brew install gradle
brew remove gradle
brew doctor

sh -c "$(curl -fsSL https://raw.githubusercontent.com/Linuxbrew/install/master/install.sh)"

switchdesk gnom-
switchdesk kde

export JAVA_HOME=/usr/share/jdk1.6.0_14 
export PATH=$JAVA_HOME/bin:$PATH 
export CLASSPATH=.:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar 

source /etc/profile

echo $JAVA_HOME

创建桌面链接，此处最好在root用户下进行
vim /usr/share/applications/eclipse.desktop
写入以下内容
[Desktop Entry]
Name=Eclipse
Comment=Eclipse SDK
Encoding=UTF-8
Exec=/usr/local/eclipse/eclipse
Icon=/usr/local/eclipse/icon.xpm
Terminal=false
Type=Application
Categories=Application;Development;
完成后可以在Application-Programming下看到eclipse图标
