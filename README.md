
# 🚀Install Apache Web Server on Ubuntu WSL and run a frontend clone of Google.com on Locahost!


The Apache HTTP server is the most widely-used web server in the world. It provides many powerful features including dynamically loadable modules, robust media support, and extensive integration with other popular software.

## Step 1 — Installing Apache
Apache is available within Ubuntu’s default software repositories, making it possible to install it using conventional package management tools.
Let’s begin by updating the local package index to reflect the latest upstream changes:
```
sudo apt update
```
Then, install the apache2 package:
```
sudo apt install apache2
```
After confirming the installation, apt will install Apache and all required dependencies.

## Step 2 — Checking your Web Server
At the end of the installation process, Ubuntu 20.04 starts Apache. The web server should already be up and running.
Check with the systemd init system to make sure the service is running by typing:
```
sudo systemctl status apache2
```
If the service in inactive, you can activate it by typing:
```
sudo systemctl start apache2
```
You can Deactivate the service by typing:
```
sudo systemctl stop apache2
```

## Step 3 — Accessing the default Apache landing page
You can access the default Apache landing page to confirm that the software is running properly through your IP address. If you do not know your server’s IP address, you can get it a few different ways from the command line.
Try typing this at your server’s command prompt:
```
hostname -I
```
When you have your server’s IP address, enter it into your browser’s address bar:
```
http://your_server_ip
```
You should see the default Ubuntu 20.04 Apache web page:
![App Screenshot](https://assets.digitalocean.com/articles/how-to-install-lamp-ubuntu-16/small_apache_default.png)

## Step 4 — Creating a Frontend Clone of Google.com
#### 🛠 Skills Required:
- HTML5
- CSS3

The codes required are already present in the apache_project folder.
Type the below commands to clone the repository and run the frontend clone of google.
Clone the project:
```
git clone https://github.com/tejasdurge55/apache2_tejasdurge_project.git
```
Go to the project directory:
```
cd apache2_tejasdurge_project/apache_project/
```
Copy the files:
```
cp google.png  index.html  package.json  picture_of_working_project.png  styles.css  vite.config.js /var/www/html/
```

You should be able to see your Google web page:
![App Screenshot](https://github.com/tejasdurge55/apache2_tejasdurge_project/blob/master/apache_project/picture_of_working_project.png?raw=true)


# Thank you👋

## 🔗 Links To Connect with Me

[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/tejas-durge-0a62a128a/)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/TejasDurge55)

