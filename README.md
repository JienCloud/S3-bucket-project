# Host a Website on Amazon S3

**Author:** Jieno Renz Cadiz  
**Email:** jienorenzcadiz@gmail.com

---

![Image](http://learn.nextwork.org/contented_white_innocent_cobra/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Introducing Today's Project!

### Project overview

In this project, I will demonstrate on making S3 bucket to host a static website, I'm doing this project to learn more about aws services and learn how to host websites.

### Tools and concepts

Services I used were S3 Bucket Key concepts I learnt include how to make storage where I can upload my website resources, how to host a static website, and how to set up rules within my bucket so no one can delete and destroy it.

### Time, challenges, and wins

This project took me approximately many minute because I am trying to understant and learn where to use it. 

---

## How I Set Up an S3 Bucket

### What I did in this step

In this step, I will now open up Amazon S3 because I will now learn how create a storage space for my website files before hosting my static website.

### How long it took to create the bucket

Creating an S3 bucket took me minutes since I am trying to understand the settings before creating a bucket to ensure that I can it can fit to my liking.

### Region selection

The Region I picked for my S3 bucket was Singapore, since im in the Philippines I chose this region because it is the closest to me. For my understanding the closer the region is to me the less will be charge into me.

### Understanding bucket name uniqueness

S3 bucket names are globally unique so that no one can use your own bucket or do anything with it. If you try to create a bucket with existing S3 bucket name then it will be blocked.

![Image](http://learn.nextwork.org/contented_white_innocent_cobra/uploads/aws-host-a-website-on-s3_ba6d42ad)

---

## Upload Website Files to S3

### What I did in this step

In this step, I will not upload files into my bucket because doing so will my website have contents in it.

### Files I uploaded

I uploaded two files to my S3 bucket - they were index.html and other files as contents.

### How the files work together

Both files are necessary for this project as one file alone such as the index.html as the structure of the website will not have any contents at all so uploading other files like images will fill the website.

![Image](http://learn.nextwork.org/contented_white_innocent_cobra/uploads/aws-host-a-website-on-s3_a265af88)

---

## Static Website Hosting on S3

### What I did in this step

In this step, I will be making my static website available to anyone but because I'm still learning I will be deleting this project but will explore later on.

### Understanding website hosting

Website hosting means putting files into web servers which is a computer that let people can take a look and visit.

### How I enabled website hosting

To enable website hosting with my S3 bucket, I went to the properties tab and scroll all the way down and enabled static website hosting and also put the index.html since this is the document that I'm trying to host.

### Access Control Lists (ACLs)

An ACL is a set of rules on who decides who can get the access to the resources for example the S3 bucket I will be creating have the ACL enabled so that I can have the previledge to access a specific object in my bucket. There is also bucket policies which is popular because its much simpler but today I'd to make my bucket with ACL to learn and explore. 

![Image](http://learn.nextwork.org/contented_white_innocent_cobra/uploads/aws-host-a-website-on-s3_c22c54c0)

---

## Bucket Endpoints

### Understanding bucket endpoint URLs

Once static website is enabled, S3 produces a bucket endpoint URL, which is also just like an ordinary url that function for people to access and visit your website url.

### What I saw when I tested the endpoint

When I first visited the bucket endpoint URL, I saw access denied or 403 Forbidden. The reason for this error was because the website or bucket are automatically private so before anyone can see the website I need to go back to  my bucket-object select my files and go to actions and make public using ACL

![Image](http://learn.nextwork.org/contented_white_innocent_cobra/uploads/aws-host-a-website-on-s3_22ce4daf)

---

## Success!

### What I did in this step

In this step, I will be making this website online and publicly accessible because for now everyone dont have any permission to visit this website.

### How I resolved the 403 error

To resolve this 403 Forbidden error, I go to back to the aws console bucket and go to objects and select all file and then go to actions and make the public. 

![Image](http://learn.nextwork.org/contented_white_innocent_cobra/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Bucket Policies

### What I did in this extension

In this project extension I'm about to set up a bucket policy. I'm doing this so that I can choose who can access and edit my bucket files.

### Understanding bucket policies

An alternative to ACLs are bucket policies, which are rules that determines who is allowed to do something in that bucket. The benefit of using bucket policies is so that you can gain more control on your own bucket and can prevent others editing your bucket, while ACLs are useful for individual access to objects in the bucket.

![Image](http://learn.nextwork.org/contented_white_innocent_cobra/uploads/aws-host-a-website-on-s3_sm2sm2sm)

### What my bucket policy does

My bucket policy is to prevent anyone from deleting the file named index.html. I tested this by trying to delete the file and saw the access denied. I also experimented the policy so that instead of blocking the file I make it so that only I can delete all the files in the bucket and others can't.

---

---
