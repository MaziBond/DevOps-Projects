# LAMP Stack Implementatin

## Launching a AWS EC2 instance 

### - lauching an EC2 instance

![EC2 successful screenshot](images/LAMP_successful_launch.png)


### - Successful running an EC2 instance

![EC2 instance running screenshot](images/LAMP_EC2_instance_screenshot.png)


### - Connect the EC2 instance using SSH

![connect to instance page screenshot](images/LAMP_connect_to_instance_Page.png)

![connect to instance screenshot](images/lamp_connect_to_instance.png)

## install Apache2
```Bash
sudo upgrade && sudo update
```
```Bash
sudo apt install apache2 
```
![apache2 installation screenshot](images/lamp_Apache2_installation.png)

### - check apache status

```Bash
sudo systemctl status apache
```
![apache status screenshot](images/Lamp_Apache_status.png)

### - Check Apache server connection to public server

```Bash
curl http://localhost:80
```

```Bash
http://<AWS public ip address>
```
![Apache working screenshot](images/lamp_Apache_network_working.png)

## Installation of MySQL

