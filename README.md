# Deploying WordPress,MySQL and PhpMyAdmin with Persistent Volumes 

Step one : 

# MYSQL Deployment: 

1.Create the service of mysql in order to lunch the mysql . 
2.Need to create the Persistant Volume for Mysql data . 
3.Creat a Deployment of mysql :
	a.Create Stragey with Recreation Method.
	b.Creat template for mysql with specfic of container along with secret key.
	c.Attached persistance volume with Container . 

step Two:

# Word Press Deployment : 

1.Create the service of wordpress  in order to lunch the Wordpress Pod with loadbalancer type.
2.Need to create the Persistant Volume for wordpress data . 
3.Creat a Deployment of Wordpress Application :
	a.Create Stragey with Recreation Method.
	b.Creat template for mysql with specfic of container along with secret key.
	c.Expose wordpress applicaiton over the internet on port 80 with help of loadbalancer.
	d.Attached persistance volume with Container with mount.
  
Step Three : 

# PhpMyAdmin Deployment : 

1.Create the service of PhpMyadmin in order to lunch the PhpMyAdmin Pod.
2.Creat a Deployment of PhpMyAdmin Application :
	a.Create Stragey with Recreation Method with replica One.
 	b.Creat template for PhpMyadmin with specfic Container name image and port .
	c. Contect phpmyadmin applicaiton with Mysql with help of ENV Variable . 

NOTE: ALL code are avaible on git hub Moreover ALL code is written in YAML LAnaguage. 

	
