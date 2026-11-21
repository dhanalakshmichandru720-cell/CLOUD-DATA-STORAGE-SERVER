# CLOUD-DATA-STORAGE-SERVER
CLOUD DATA STORAGE SERVER
 CLOUD-DATA-STORAGE-SERVER

### NAME : Dhanalakshmi c
### REG NO: 212225230050

## Aim

To create and configure an Amazon Relational Database Service (Amazon RDS) instance as a cloud data storage server, configure the required security settings, connect it to a web application, and perform database operations using the application.

## Algorithm / Steps

1. Create a Security Group for the RDS database.
2. Add an inbound rule to allow MySQL (Port 3306) access from the Web Security Group.
3. Create a DB Subnet Group using two Availability Zones.
4. Launch an Amazon RDS MySQL database instance.
5. Configure the database with the required identifier, username, password, storage, and instance class.
6. Associate the database with the created Security Group and Subnet Group.
7. Wait until the database status becomes **Available**.
8. Copy the RDS endpoint.
9. Open the web application u
10.  the provided Web Server IP address.
10. Enter the RDS endpoint, database name, username, and password.
11. Connect the application to the database.
12. Verify the connection by adding, editing, and deleting records in the Address Book application.


## Program

### Security Group Configuration

* Security Group Name: **DB Security Group**
* Inbound Rule: **MySQL/Aurora (3306)**
* 
* Source: **Web Security Group**
* ### DB Subnet Group

* Name: **DB-Subnet-Group**
* VPC: **Lab VPC**

### Amazon RDS Configuration

* Engine: **MySQL**
* Template: **Dev/Test**
* Availability: **Multi-AZ**
* DB Instance Identifier: **lab-db**
* Username: **main**
* Password: **lab-password**
* Instance Class: **db.t3.micro**
* Storage: **20 GB (Ge
* neral Purpose SSD)**

### Connect the Application

```text
Endpoint : <RDS Endpoint>
Database : lab
Username : main
Password : lab-password
```
After submitting the above details, perform Add, Edit, and Delete operations on the Address Book application.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8be349ae-cf99-4eb2-b774-5168cf367979" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0e79f6e8-40c4-4147-ac41-48dadadd1ce0" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0cff7bab-f2c3-4f08-b940-f79789d89d9d" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c2e40511-699f-4a97-83d6-f0795e03a149" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/899373b9-23a6-4a53-861d-dafde7b35826" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7bc91084-0a70-40c3-a334-8a14de949091" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/14cda48e-f04c-483f-8336-2ca405082159" />

## Result

Thus, an Amazon RDS database instance was successfully created and configured as a cloud data storage server. The database was securely connected to a web application, and data operations such as inserting, updating, and deleting records were successfully performed through the application.


