# Udacity_Project-5 (capstone)
Description:The  project deploys  index.html  using RollingUpdate 

*********************************************************************************************************************

Technologies Used:
===================

Docker 

Kubernetes

CircleCI

GitHub

AWS

***********************************************************************************************************************

Steps:
========

1)Test the  code using linting

2)Create an Docker image for this  Application

3)Upload the Docker image into  Docker Hub

4)Create Kubernetes cluster in AWS 

5)Create loadbalancer and web hosts for  high availability

6)Deploy container

7)Update the  web page  (Changed the version, Colour, background and format )

8)Using RollingUpdate method  deployed  this  app  again 

9)the entire  process  is run via CIRCLECI and  code is  plulled from  github repo






==========
accelorometer
=================

CREATE EXTERNAL TABLE IF NOT EXISTS `stedi`.`accelerometer_landing` (
`user` string,
`timeStamp` bigint,
`x` float,
`y` float,
`z` float
)
ROW FORMAT SERDE 'org.openx.data.jsonserde.JsonSerDe'
WITH SERDEPROPERTIES (
'ignore.malformed.json' = 'FALSE',
'dots.in.keys' = 'FALSE',
'case.insensitive' = 'TRUE',
'mapping' = 'TRUE'
)
STORED AS INPUTFORMAT 'org.apache.hadoop.mapred.TextInputFormat' OUTPUTFORMAT 'org.apache.hadoop.hive.ql.io.HiveIgnoreKeyTextOutputFormat'
LOCATION 's3://shivas-stedi-lakehouse/accelerometer/landing/'
TBLPROPERTIES ('classification' = 'json');

*********************************************************************************************************************

URLS -- URL.txt  

contains  github and   website url

Screenshots available in Screenshots folder
