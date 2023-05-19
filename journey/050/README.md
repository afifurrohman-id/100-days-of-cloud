# Meet 6 | EBS, AMI

## Cloud Research

### EBS (Elastic Block Store)

- Create Instance
  ![image](https://user-images.githubusercontent.com/118882411/223052379-346bea16-bc8f-4cca-ac4a-b3736a9b4c35.png)
- in network setting for subnet try to use other availability zone
  ![image](https://user-images.githubusercontent.com/118882411/223054202-e38634ba-7521-4e17-b578-fe315cf68dfb.png)
- After finish, click launch instance
  ![image](https://user-images.githubusercontent.com/118882411/223054644-6d05a3fe-52b0-4f52-a236-fa3ff23126b8.png)
- After finish, confirm the availability zone
  ![image](https://user-images.githubusercontent.com/118882411/223055668-7c00ec70-dfb1-4d5d-951a-4ef8c5925ad7.png)
- Go to tab Volume
  ![image](https://user-images.githubusercontent.com/118882411/223055964-a332f9e8-7564-4df7-98c5-e3340d4752eb.png)
- click create volume
  ![image](https://user-images.githubusercontent.com/118882411/223056194-7cdb0e1a-d553-4986-98a8-2d0e04b3ae2e.png)
- choose volume size & availability zone your EC2 Instance (THIS IMPORTANT!!)
  ![image](https://user-images.githubusercontent.com/118882411/223056760-94628f2b-8f98-4738-81dd-5442cc3b3233.png)
- click create volume
  ![image](https://user-images.githubusercontent.com/118882411/223056921-317d74fe-cfc0-45a7-afde-6c61bcbd847c.png)
- select your volume and click actions
  ![image](https://user-images.githubusercontent.com/118882411/223057259-ace612a0-89db-4747-8837-fa1e945a29a3.png)
- click attach volume
  ![image](https://user-images.githubusercontent.com/118882411/223057742-28fa3499-7fd4-4851-b770-c79185f3a46e.png)
- Select your instance and click attach volume
  ![image](https://user-images.githubusercontent.com/118882411/223058024-a86002b8-43bc-461a-b74f-9d9a7a78cf94.png)
- Confirm by view volume state & view in your instance storage menu
  ![image](https://user-images.githubusercontent.com/118882411/223058390-38d26df4-2d52-4f20-ba7d-5a96c15edd43.png)
  ![image](https://user-images.githubusercontent.com/118882411/223059025-1ea73a89-e849-446a-abad-8adee28ea3f4.png)
- Next try to create other instance & in the subnet select another availability zone
  ![image](https://user-images.githubusercontent.com/118882411/223059600-86ddbd36-fdfe-4b90-9914-2e50dc45c940.png)
- Confirm your instance availability zone
  ![image](https://user-images.githubusercontent.com/118882411/223061064-d31cc2ab-351d-4214-9868-a060ba897ba2.png)
- Go to volume tab and detach your volume first
  ![image](https://user-images.githubusercontent.com/118882411/223062006-80adfca5-7b32-44dc-99eb-c5855e2fc007.png)
- After that click actions to your volume and click create snapshot
  ![image](https://user-images.githubusercontent.com/118882411/223062343-efc04e8c-2229-4761-b67c-5c58730638cc.png)
- and click create snapshot
  ![image](https://user-images.githubusercontent.com/118882411/223062604-c4fb41b0-6bd5-4594-8111-c85d838727ed.png)
- go to snapshot tab
  ![image](https://user-images.githubusercontent.com/118882411/223062853-d1c0a3fd-af24-400f-8aa4-0daf5c412557.png)
- select your snapshot, click action and select create volume from snapshot
  ![image](https://user-images.githubusercontent.com/118882411/223063612-e8a72ba7-3de6-4814-b34d-6c0d4d0e505c.png)
- select availability zone (same as your instance)
  ![image](https://user-images.githubusercontent.com/118882411/223064091-7aca1eae-3199-4148-b36e-96ba210598ae.png)
- go back to volume and attach your volume from snapshot
  ![image](https://user-images.githubusercontent.com/118882411/223064368-e7570148-97d8-4292-8103-b457240481a6.png)
- select your instance and click attach
  ![image](https://user-images.githubusercontent.com/118882411/223064567-c7b196f9-553e-4fe8-b8f5-ede779503378.png)
- confirm by view in storage tab in your instance
  ![image](https://user-images.githubusercontent.com/118882411/223064788-b6fcecd1-63cf-4567-9605-8e6e26d1f993.png)

### AMI (Amazon Machine Image)

- First Create new Instance & in security group Allow traffic from http (or use your security group in same rule)
  ![image](https://user-images.githubusercontent.com/118882411/223068282-d54b5b4a-0d26-4451-be09-1a045468c111.png)
- In your user data use script to start your web server app & click launch instance
  ![image](https://user-images.githubusercontent.com/118882411/223069110-3c2bf917-8275-4d3e-b012-7b4060ecdcfd.png)

- After finish, copy your dns url and paste in your browser to confirm
  ![image](https://user-images.githubusercontent.com/118882411/223070329-736a4db7-9db5-4540-acfe-1939c6e70633.png)
- Look like this
  ![image](https://user-images.githubusercontent.com/118882411/223070630-3f535eab-5079-4aea-a5e0-f1105908370e.png)
- Select your instance, right click and select images & templates > Create Images
  ![image](https://user-images.githubusercontent.com/118882411/223071032-06050c78-9b20-4863-b6e0-15f6c65e1d2c.png)
- enter name for image & click create image
  ![image](https://user-images.githubusercontent.com/118882411/223071346-44b8efcc-ad7d-4fe4-8430-7b70cdbccadf.png)
- go to AMIs tab and select your image, click launch instance from AMI
  ![image](https://user-images.githubusercontent.com/118882411/223071765-5b9335f5-4f2a-4893-b4b7-1e36ca4ebf08.png)
- in applications and os image select your ami
  ![image](https://user-images.githubusercontent.com/118882411/223072302-be4d8af5-6ce6-477e-8f57-79d47e1fef3d.png)
- select your security group to allow http traffic
  ![image](https://user-images.githubusercontent.com/118882411/223072525-ed2c376d-aacd-4445-9d77-31635c03803c.png)
- add script to create html files & click launch instance
  ![image](https://user-images.githubusercontent.com/118882411/223073478-217efc78-28dd-4f17-aace-b456876eb5a5.png)
- copy your public dns in your instance & paste in your browser
  ![image](https://user-images.githubusercontent.com/118882411/223079245-ccd82ba3-480a-4de2-9b34-06c6db4f5c97.png)
- and done
  ![image](https://user-images.githubusercontent.com/118882411/223079435-29d4d446-9039-46f5-a6cf-5a59af3e9fba.png)

## Next Steps

-
