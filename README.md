# Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu

## AIM

To implement Pseudo Node configuration for Hadoop on ubuntu

## Pre-requisites

a) jdk

Single-Node Configuration

1.	Create a dedicated user account for hadoop

2.	![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/893806be-64df-40d0-aca2-6edbfb2c8cbd)

   

3.	Install java1.8 in folder /usr/local

4.![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/f3563662-962c-40cd-bae0-9622193cf5e5)

   
5.	Install Hadoop

6.	![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/2d3559cf-1788-4718-af68-fa46645772d3)


7.	Set the hadoop environment variables: Include the following lines in the
$HOME/.bashrc file

![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/b9937399-83e5-42fa-bac6-ea76c8ca6fe5)


 
9.	Set hadoop environment variables: Include the following lines /etc/profile file

10.	![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/1f1446b8-07ab-4c04-9527-d992430ac9d1)



11.	Run the.bashrc & profile files from the $ prompt for updating the changes

![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/303adce4-ad4e-46a2-baf9-bc6f5e156309)

![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/00d0f13f-4dab-4dc0-a9bb-13117bf44eac)


$ bin/hadoop version	

7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml

path ::	/usr/local/hadoop-2.5.1/etc/hadoop

a)	hadoop-env.sh
Include the following lines in hadoop-env.sh file

![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/2e0c7f2e-3611-45a4-a3ae-33ea008f9379)



b)	core-site.xml
Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)

![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/b4606ce0-caf9-41d9-a4d2-590353818b53)



 
Include the following lines in core-site.xml file between <configuration> and
</configuration> tags

![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/777ee591-941c-420a-8b73-59981b8006a3)



c)	mapred-site.xml

![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/d327e5bb-eb88-4f8c-a6f7-9a6c31525c7e)


 

Include the following lines in mapred-site.xml file

![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/e1c9486a-21cc-4879-aa61-a3180a3b54dd)

 

d)	hdfs-site.xml
Include the following lines in hdfs-site.xml file

![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/bf4c43e6-650d-4938-a46a-c52cb75e04f6)


e)	yarn-site.xml
Include the following lines in yarn-site.xml file

![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/d8f044de-d6e3-4418-b9a7-0703ba66879a)

8.	Format the Hadoop File system implemented on top of the local file system using

9.	![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/4455e284-c983-48f6-bbe4-589653985cb6)


10.	Start Hadoop using

11.	![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/3f807d8a-b49d-4c66-9ed2-5797091ca102)



Explore Hadoop using http://localhost:50070/ from the browser	
 
10.	The commonly used HDFS Commands are as follows:

11.	![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/d0120611-5f35-45d6-81f8-809574255194)



12.	Create a directory ‘/input’ in HDFS

13.	![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/1fc6f996-d885-425c-812a-76095abd716f)



14.	Copy the input files into the distributed file system

15.	![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/bee69dd3-9b73-4438-8181-d80bcdcd1e32)


16.	Run some of the examples provided

17.	![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/04122f6b-b0e6-42a1-9766-764de3fc370c)



18.	Examine the output files

19.	![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/11e6d9d7-37b2-43e2-9ead-bdd937e9775e)

Copy the output files from the distributed file system to the local file system and examine them:

![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/970c0f00-e1d0-4506-8836-769a44eed881)

 
or
View the output files on the distributed file system

![image](https://github.com/chgeethika/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209368/73ceb3a9-def5-4d0f-a223-b545f11ab09f)


## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
