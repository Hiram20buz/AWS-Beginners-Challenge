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

## Step 5: Upload Your Website Files

In the **General purpose buckets** section:

1. Click on your newly created bucket.  
2. Prepare your website files:  
   - An **HTML file** (the main page of your site).  
   - An **images folder** (unzipped).  
3. Upload both the HTML file and the images folder into your S3 bucket.  
   > ⚠️ Do not upload the ZIP file directly — make sure you upload the extracted folder instead.

![Upload Files](https://github.com/user-attachments/assets/969fc3f1-f97e-4749-86bf-c767f000552b)

## Step 6: Enable Static Website Hosting

1. Open your S3 bucket settings:  
   - Go to the **Properties** tab.  
   - Scroll to **Static website hosting** and click **Edit**.  
   - Enable hosting, choose **Host a static website**, and set **index.html** as the default page.  

![Enable Static Hosting](https://github.com/user-attachments/assets/8d4f7966-7e7f-4dfd-8730-0b770f6c20e3)

2. Once saved, you’ll see a **public website endpoint**.  
   - Copy this link and open it in your browser to view your hosted site.  

![Website Link](https://github.com/user-attachments/assets/5a74feb6-c04e-4c9d-846c-b24570e00965)

## Step 7: Make objects in your S3 bucket public
1-Make your website files in S3 publicly accessible
2-See your website live on the internet
