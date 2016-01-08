# Android Login and Registration with PHP, MySQL and SQLite

#####VIDEO DEMO

[![Android Login and Register Youtube Video](http://img.youtube.com/vi/tLxlR7l_jH4/0.jpg)](http://www.youtube.com/watch?v=tLxlR7l_jH4)


######Creating MySQL Database and Tables

    create database android_api /** Creating Database **/
     
    use android_api /** Selecting Database **/
 
    create table users(
       id int(11) primary key auto_increment,
       unique_id varchar(23) not null unique,
       name varchar(50) not null,
       email varchar(100) not null unique,
       encrypted_password varchar(80) not null,
       salt varchar(10) not null,
       created_at datetime,
       updated_at datetime null
    ); /** Creating Users Table **/
    
    
######Creating PHP Project

Goto the location where wamp installed and open www folder. The default installation location of wamp would be C:/wamp. Below is the final PHP project structure we are going to create in this article.
    
    
