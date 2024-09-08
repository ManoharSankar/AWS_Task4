# AWS_Task4
To create and attach an Elastic Block Store (EBS) volume to an instance in Amazon Web Services (AWS), you can follow these steps:

Step 1: Create an EBS Volume
Login to AWS Management Console:

Open the AWS Management Console and log in with your credentials.
Navigate to the EC2 Dashboard:

From the AWS Management Console, choose Services > EC2.
Create a New Volume:

On the left sidebar, click on Volumes under the "Elastic Block Store" section.
Click Create Volume.
Configure Volume Specifications:

Volume Type: Choose a volume type (e.g., gp3 for General Purpose SSD, io1 for Provisioned IOPS SSD, st1 for Throughput Optimized HDD).
Size: Specify the size of the volume in GiB.
Availability Zone: Select the same Availability Zone as your EC2 instance (EBS volumes can only be attached to EC2 instances within the same Availability Zone).
IOPS: If using io1 or io2 volume types, specify the number of IOPS.
Encryption: Choose whether the volume should be encrypted and, if so, select the key for encryption.
Create the Volume:

Click Create Volume. The new volume will now appear in the list of EBS volumes.
Step 2: Attach the EBS Volume to an EC2 Instance
Select the Newly Created Volume:

From the Volumes page in the EC2 Dashboard, find the volume you just created and click on it to select it.
Attach the Volume:

Click Actions > Attach Volume.
Configure Attachment Settings:

Instance: Select the EC2 instance you want to attach the volume to. Make sure this instance is in the same Availability Zone as the volume.
Device: Choose the device name for the volume (e.g., /dev/sdf, /dev/xvdf). AWS will automatically provide a device name if you don't specify one.
Attach the Volume:

Click Attach Volume. The volume will be attached to the instance.
