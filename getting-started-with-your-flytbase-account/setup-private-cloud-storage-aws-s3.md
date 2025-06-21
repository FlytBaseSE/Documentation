---
description: >-
  Follow the instructions in this guide to set up your private cloud storage
  using AWS S3 and enable media storage on a secure Cloud for your autonomous
  BVLOS drone operations.
---

# Setup Private Cloud Storage (AWS S3)

FlytBase supports the upload and storage of media captured during drone operations in a private Amazon S3 bucket. Click [here](https://aws.amazon.com/s3/) to learn more about Amazon S3, and follow the instructions below to set up your own S3 bucket.

### Step 1:  Create/ Sign in your AWS Account

Sign in to your AWS Account here: [https://aws.amazon.com/.](https://aws.amazon.com) Click on **Create an Account** if an account does not exist.

### Step 2: Create Bucket

Go to the **Bucket** tab in the Amazon S3 console. Click on **Create Bucket** to create a bucket in the preferred region.

<figure><img src="https://lh7-us.googleusercontent.com/qFveXsoUSxiKXQ0hhMXvimBau8hWdYMAAkA8joYFBEiSmZl6PPoH-6zdFH_qy2tEeHo4wHBHo2eTubsJyhLOAAOgczg8vZn9EKRZn3s1V3P2tiouq6cLWOZIgFnc5KPPTS8nIQOAfX3rDogn4zg7tp4" alt=""><figcaption><p>Create a Bucket in the Amazon S3 Console</p></figcaption></figure>

### Step 3: ACL and Object Ownership

Click on **ACLs Enabled** and select the Object Ownership to **Bucket owner preferred**.

<figure><img src="https://lh7-us.googleusercontent.com/5_23McLv0llTvCecrgBpXE31AdArmvXLFy3EMEaWAQwZUvplAwWtEJsUprTiaKBgCFCggVjkZ-30vTgQwC84HQRFFwDeD7U393rV2fDI9vOY5-BVe-UzYS4-AHYRJFz_lNRhOU60Hiac5qzIKuu2H08" alt=""><figcaption><p>Selected options under the Object Ownership tab</p></figcaption></figure>

### Step 4: Edit Block Public Access

Under the **Edit Block public access** tab, enable **Block&#x20;**_**all**_**&#x20;public access** by checking the square box.

<figure><img src="https://lh7-us.googleusercontent.com/zJGwbcp4N62WAHspcgtJzr2llXa-MGLHyIaCvSXM106RmqDHSRihJbCIN5_5cR0zHrJTNllN0w9sXNpgFYOWWBlgWfq7XhEwxxqGmfAu_6TsS2S824KX-o3envJzIJ-510apEI9w4a65LOK3RQST2jk" alt=""><figcaption><p>Edit Block public access tab</p></figcaption></figure>

### Step 5: Bucket Versioning

Under the **Bucket Versioning** tab, click on **Disable**.

<figure><img src="https://lh7-us.googleusercontent.com/GQfURsaO9i6ea7Kl88Dg_OQK4uQQiFxU4Z5MW8M69x7ob0T63gv_KU4fhjBNz0LZtaQ2JE4AZKuyulc2pEPh6t7uH6pE0nJMDCOMLBoXGDqUlyjT-oSNRKKsmcE9k02t6spxu_AEUZCGRSQGyRfy64c" alt=""><figcaption><p>Bucket Versioning tab</p></figcaption></figure>

### Step 6: Configuring Default Encryption

Now, under the Default Encryption tab, set the following options:

* For **Encryption type**, select **Server-side encryption with Amazon S3 managed keys (SSE-S3)**
* Set **Bucket Key** to **Enable**

Set the Encryption type to Server-side encryption with Amazon S3 managed keys (SSE-S3) and Bucket Key to Enable.

<figure><img src="https://lh7-us.googleusercontent.com/jtvZcp6QyCJwjeHgdtrPY54OB3N0THntd6xLtJ1pvXeHIaTJU9JMwHU86uPrNQAewQ796xUajxdsmvEqEZx3hXbvtcd9fNzWDd5IS5ifYKPe8OrfXcbas3M2O5stC_aLDGBjWhrWNwcXRz3OG96JWko" alt=""><figcaption><p>Default Encryption tab</p></figcaption></figure>

### Step 7: Enable Transfer acceleration

Once the Bucket has been successfully created, navigate to **Bucket Name** -> **Properties** -> **Transfer acceleration** and edit it to **Enabled**.

<figure><img src="https://lh7-us.googleusercontent.com/NJshSPFHSTAlISIirPX-LtPdS5HznDX-pY6Kz1povJMXs5sxBkgWsRdiaXqsXWFNH2LR2meJxQ7MXDWZQqyFCDdqButmPYNonQq7_Q_T6qM9c3AIYnY3HsVvBCMrlrNhkNeECR4bTAztljJdvrxbRAE" alt=""><figcaption><p>Transfer acceleration set to enabled</p></figcaption></figure>

### Step 8: Editing Bucket Policy

Navigate to **Bucket Name** -> **Permissions** -> **Bucket Policy**. Paste the following JSON code snippet, and replace **Bucket\_Name** with the actual name of the Bucket.

```json
{
    "Version": "2012-10-17",
    "Id": "Policy1586431420805",
    "Statement": [{
        "Sid": "Stmt1586431413927",
        "Effect": "Allow",
        "Principal": {
            "AWS": "arn:aws:iam::805060674250:user/storage-flytbase"
        },
        "Action": "*",
        "Resource": [
            "arn:aws:s3:::Bucket_Name",
            "arn:aws:s3:::Bucket_Name/*"
        ]
    }]
}
```

### Step 9: Update CORS Configuration

Now, proceed to **Bucket Name** -> **Permissions** -> **CORS Configuration**. To update the CORS Configuration, you will need your FlytBase Organization URL.&#x20;

For instance, if your Organization's URL is **org\_sub\_domain.flytbase.com**, then update the **AllowedOrigins** array as follows:

```
[
    {
        "AllowedHeaders": [
            "*"
        ],
        "AllowedMethods": [
            "GET"
        ],
        "AllowedOrigins": [
            "https://org_sub_domain.flytbase.com/*"
        ],
        "ExposeHeaders": [],
        "MaxAgeSeconds": 1800
    }
]

```

### Step 10: Inform FlytBase Support for S3 Bucket Activation

Once you have completed all the steps, please share the **Bucket Name** and the **AWS Region ID** to [support@flytbase.com](mailto:support@flytbase.com). Our Support team will then link your AWS S3 Bucket to your Organization.

***

After creating your Organization, and linking an AWS S3 Bucket to it, the media files captured during flights will be uploaded to your private cloud storage automatically.
