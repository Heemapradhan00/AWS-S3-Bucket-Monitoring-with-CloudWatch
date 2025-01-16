# AWS S3 Bucket Monitoring with CloudWatch

This project demonstrates how to set up server access logging for an S3 bucket and use AWS CloudWatch to track and alert when a new object is uploaded. 

## Features
- Enable server access logging for S3 buckets.
- Configure CloudWatch event rules for real-time notifications.
- Integrate with SNS for email alerts.

## Prerequisites
- An AWS account.
- Basic knowledge of AWS services like S3, CloudWatch, and SNS.

## Steps to Implement

### Step 1: Enable Server Access Logging
1. Log in to the AWS Management Console and navigate to the **S3** service.
2. Create a new bucket or use an existing one.
3. Go to the **Properties** tab of the bucket.
4. Scroll to **Server access logging** and enable it.
5. Set the destination bucket for logs and save changes.

### Step 2: Configure CloudWatch Event Rules
1. Open **CloudWatch** in the AWS Management Console.
2. Navigate to **Rules** under the Events section.
3. Create a new rule:
   - Event source: AWS Services → S3.
   - Event type: All Events.
4. Add a JSON filter for the S3 bucket you want to monitor.
5. Set the target to **SNS** and configure an email subscription.
6. Confirm the email subscription.
7. Test the setup by uploading an object to the S3 bucket.

## Notifications
- Receive real-time email notifications whenever an object is uploaded to the S3 bucket.

## License
This project is licensed under the MIT License.
![image](https://github.com/user-attachments/assets/c69dec4a-ee82-4a75-ab28-9004eb2eb7e3)

