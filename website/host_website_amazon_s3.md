# Hosting a Static Website on Amazon S3

## Step 1: Open the S3 Service
Log in to the [AWS Management Console](https://console.aws.amazon.com/) and navigate to **Amazon S3**.

![Open S3](https://github.com/user-attachments/assets/b7ec369c-d243-4e54-ba19-92b1663b3905)

---

## Step 2: Select the Closest Region
Choose the **AWS region** that is geographically closest to you to reduce latency and costs.  
For example, users in **Tijuana, Mexico** should select **Norte de California (`us-west-1`)**.

![Choose Region](https://github.com/user-attachments/assets/3c890715-bc05-4c4b-a2f3-db19ed178ff0)

## Step 3: Create a New Bucket
Click on **Create bucket** to start setting up a new S3 bucket where your website files will be stored.

![Create Bucket](https://github.com/user-attachments/assets/5db496fa-244c-40bf-a6c2-d7a2a2fc9f3b)

## Step 4: Configure Your New Bucket

Fill in the required settings for your bucket:

1. **Bucket name** – Choose a unique name (S3 bucket names must be globally unique).  
2. **Object ownership** – Select **ACLs enabled** and set the preferred bucket owner.  
3. **Public access settings** – **Uncheck** “Block all public access” so the bucket can serve website files.  
4. **Bucket versioning** – Enable versioning to keep track of file changes.  
5. Leave all other options as default.  

Finally, click **Create bucket** to complete the setup.

![Bucket Setup](https://github.com/user-attachments/assets/65757505-e5d0-404d-a441-09f6662f02ef)

## Step 5: Upload website content to your bucket
In the General purpose buckets section:
1-Click on the bucket
2-Download an HTML file that sets up your website.
3-Download a zip file of images for your website.
4-Upload both files into your S3 bucket.
