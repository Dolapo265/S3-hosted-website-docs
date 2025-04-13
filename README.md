<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Host a Website on Amazon S3

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-host-a-website-on-s3)

**Author:** dolaposalaam@outlook.com  
**Email:** dolaposalaam@outlook.com

---

![Image](http://learn.nextwork.org/sincere_violet_daring_manta_ray/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Introducing Today's Project!

In this project, I’ll show how to host a static website using an Amazon S3 bucket. My goal is to learn the basics of cloud hosting and gain hands-on experience with AWS.

### Tools and concepts

The service I used was Amazon S3. Key concepts I learned include ACLs vs. bucket policies, static website hosting, object storage, and public access settings.

### Project reflection

This project took me about 2 hours to complete. The most challenging part was uploading the files correctly. The most rewarding part was encountering 403/404 errors and troubleshooting them successfully.

---

## How I Set Up an S3 Bucket

Creating an S3 bucket took me 2 minutes. The most challenging part was making the name unique 

The Region I picked for my S3 bucket was eu-west-2 because this is the region closest to me. 

S3 bucket names must be globally unique, meaning no other bucket across all of AWS can have the same name.

![Image](http://learn.nextwork.org/sincere_violet_daring_manta_ray/uploads/aws-host-a-website-on-s3_ba6d42ad)

---

## Upload Website Files to S3

### index.html and image assets

I uploaded two files to my S3 bucket:  the index.html file and another file containing all the images used on the site. 

Both files are necessary for this project: the index.html file defines the structure and layout of the website, while the images file contains all the images used. Without these, images may not display correctly, and errors could occur.

![Image](http://learn.nextwork.org/sincere_violet_daring_manta_ray/uploads/aws-host-a-website-on-s3_a265af88)

---

## Static Website Hosting on S3

Website hosting allows my S3 bucket can act as a webserver giving aceess to and displaying the index.html file and images uploaded  via a public UR.

To enable website hosting with my S3 bucket, I navigated to the properties tab and enabled static website hosting. 

An ACL consists of rules that determine who can access the individual objects(website files) within my bucket.

![Image](http://learn.nextwork.org/sincere_violet_daring_manta_ray/uploads/aws-host-a-website-on-s3_c22c54c0)

---

## Bucket Endpoints

Once static website hosting is enabled, S3 generates a bucket endpoint URL, which is a link that allows anyone to access the contents of the S3 bucket on a webpage

When I first visited the bucket endpoint URL, I encountered a 403 error. This occurred because, while the bucket was public, the contents were private and could not be accessed or displayed.

![Image](http://learn.nextwork.org/sincere_violet_daring_manta_ray/uploads/aws-host-a-website-on-s3_22ce4daf)

---

## Success!

To resolve this 403 Forbidden error, I made all my objects public using ACL 

![Image](http://learn.nextwork.org/sincere_violet_daring_manta_ray/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Bucket Policies

---

---
