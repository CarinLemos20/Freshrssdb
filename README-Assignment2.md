# Assignment 2: DynamoDB & Python API Deployment

## Architecture & Security
* Deployed a lightweight Python/Flask web application on an Ubuntu EC2 instance.
* Provisioned an Amazon DynamoDB NoSQL table (`StudentDirectory`).
* **Security:** Attached an IAM Role (`EC2-DynamoDB-Role`) directly to the EC2 instance, allowing passwordless, secure API access to DynamoDB.

## Database Schema & Datatypes
The NoSQL table uses `student_id` (String) as the Partition Key. It successfully implements 5 DynamoDB attribute types:
1. **String (S):** `student_id`, `name`
2. **Number (N):** `age`, `gpa`
3. **Boolean (BOOL):** `is_enrolled`
4. **List (L):** `enrolled_courses`
5. **Map (M):** `address`
