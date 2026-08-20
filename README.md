# Freshrssdb
# Lab 1: FreshRSS Database Deployment

## Database Deployment Steps (AWS RDS)
1. Created a new PostgreSQL instance in AWS RDS (Free Tier).
2. Configured the master username and password.
3. Created a strict Security Group (`RDS-Security-Group`) attached to the database.
4. Set the initial database name to `freshrss`.

## Connection Steps
1. Deployed an Ubuntu EC2 instance and installed Apache, PHP, and FreshRSS.
2. Updated the `RDS-Security-Group` inbound rules to only accept PostgreSQL (Port 5432) traffic from the EC2 instance's Security Group.
3. Accessed the FreshRSS web setup via the EC2 Public IP.
4. Entered the RDS Endpoint URL, username, and password into the FreshRSS database configuration screen to establish the connection.
