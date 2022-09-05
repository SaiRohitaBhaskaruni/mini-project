# mini-project

sudo su  --> allows you to change to root user
yum update -y   --> update our ec2 instance
yum install -y httpd  --> download apache on ec2 instance
cd /var/www/html   --> change directory to html directory ( go to html folder ) 
wget https://github.com/azeezsalu/techmax/archive/refs/heads/main.zip   --> wget is the linux command you can use to download a file to your ec2 instance, once wget is typed you have to type url tp where the file you are trying to download is located
unzip main.zip
cp -r techmax-main/* /var/www/html/
rm -rf techmax-main main.zip
systemctl enable httpd 
systemctl start httpd
