# Meet 7 | Application Load Balancer, Auto Auto Scaling Groups

## Cloud Research

### Application Load Balancer

- First create instance & and use security groups to allow http
  ![image](https://user-images.githubusercontent.com/118882411/224490493-7fb561a5-8321-4349-92ea-4fa61aeca460.png)
- Insert user data & number of instance
  ![image](https://user-images.githubusercontent.com/118882411/224490861-1e2f4f83-13c8-4b54-bdfb-17286e5ce615.png)
- confirm finished create instance
  ![image](https://user-images.githubusercontent.com/118882411/224492165-40aa976f-3b24-4a34-b1a2-fd33a5a8b8a7.png)
- Go to load balancer tab and click create load balancer
  ![image](https://user-images.githubusercontent.com/118882411/224492208-8cb116d1-3625-492e-900c-dceb2f1b84b5.png)
- select app load balancer
  ![image](https://user-images.githubusercontent.com/118882411/224492287-8a1d86ab-2d9c-4531-9029-ca3c57d36a58.png)
- in mapping checked all availability zone
  ![image](https://user-images.githubusercontent.com/118882411/224492365-341adce1-c0c9-4276-a4fc-f5d8f0ba96d8.png)
- select security group allow http
  ![image](https://user-images.githubusercontent.com/118882411/224494820-cbd841ac-3f00-4045-b2c8-e2d0bc1120e1.png)
- In listener & routing select create target group
  ![image](https://user-images.githubusercontent.com/118882411/224492447-dfd6b317-cce5-48a1-a721-9a13d5763ef3.png)
- basic config, select instance
  ![image](https://user-images.githubusercontent.com/118882411/224492528-d52aa7c9-84c2-4421-8a8d-f488f907961b.png)
- select vpc
  ![image](https://user-images.githubusercontent.com/118882411/224492559-bfe9371d-6170-4239-8cbb-bdde8254a877.png)
- interval 30s & next
  ![image](https://user-images.githubusercontent.com/118882411/224492611-c2ec6ddb-7a9d-487a-9bc3-b1b0cd8fd093.png)
- select instance & click include as pending below
  ![image](https://user-images.githubusercontent.com/118882411/224492682-4256b9e1-975e-4f14-8211-94ed41b75252.png)
- confirm
  ![image](https://user-images.githubusercontent.com/118882411/224492877-49f5e70f-009f-4785-a7ed-a51c7941926e.png)
- Back to load balancer and select target group
  ![image](https://user-images.githubusercontent.com/118882411/224492967-631baa7b-5bfc-41dd-bfa8-a56974affe37.png)
- click create load balancer
  ![image](https://user-images.githubusercontent.com/118882411/224493055-c091b581-6a32-4f85-8ad5-ec089ab8fc80.png)
- confirm
  ![image](https://user-images.githubusercontent.com/118882411/224493209-07106a57-f649-4454-9c1b-e8562e8d1854.png)
- copy your load balancer dns
  ![image](https://user-images.githubusercontent.com/118882411/224493361-a2b6b2e9-6853-4fe2-a3cc-691a73e829e8.png)
- paste in your browser
  ![image](https://user-images.githubusercontent.com/118882411/224494864-5526965f-a918-462d-9eee-68bad9d5fc2c.png)
- Test by refresh your browser
  ![image](https://user-images.githubusercontent.com/118882411/224494959-fe010e1a-6ae2-40db-9531-bcd2e5c943bf.png)

### Auto Scaling Group

- Go to auto scaling group tab and click create auto scaling group
  ![image](https://user-images.githubusercontent.com/118882411/224495376-25ef003c-cd68-459a-988a-dfb46ab0caf8.png)
- click create a launch template
  ![image](https://user-images.githubusercontent.com/118882411/224495329-748ccddf-f5f8-4a80-bfde-5bec886ae030.png)
- select os
  ![image](https://user-images.githubusercontent.com/118882411/224495696-13275756-8279-41e9-9696-959edaab3126.png)
- network setting allow http
  ![image](https://user-images.githubusercontent.com/118882411/224495729-3b65f49f-87f0-44c0-8d4e-676849e1987c.png)
- user data to start web server and click create launch template
  ![image](https://user-images.githubusercontent.com/118882411/224495806-4fb1481d-4690-4ff4-a707-7fa068baa915.png)
- back to auto scaling group and select template, click next
  ![image](https://user-images.githubusercontent.com/118882411/224495903-36a3ff22-bb45-4e9b-9c50-39b0925972bd.png)
- checked all availability zone, click next
  ![image](https://user-images.githubusercontent.com/118882411/224495975-0d24374f-4061-4d2b-96f8-cbf742885f0d.png)
- select to use load balancer
  ![image](https://user-images.githubusercontent.com/118882411/224496035-7dd040b3-2472-4e06-b09a-5d34653de01f.png)
- check elb
  ![image](https://user-images.githubusercontent.com/118882411/224496057-6156530f-651e-4759-a5c2-9b348ceefa99.png)
- group size
  ![image](https://user-images.githubusercontent.com/118882411/224496270-75af1cd6-fbf0-4333-848f-a711264aa5ef.png)
- next
  ![image](https://user-images.githubusercontent.com/118882411/224496292-e427815b-b2f4-4f85-80d2-9a09b1c4670a.png)
- next again
  ![image](https://user-images.githubusercontent.com/118882411/224496333-c7093940-0520-4882-b162-5bf51a024b0a.png)
- next
  ![image](https://user-images.githubusercontent.com/118882411/224496363-a0991b0f-6642-461c-a7c3-fd7a63aa9dfe.png)
- click create auto scaling group
  ![image](https://user-images.githubusercontent.com/118882411/224496394-0cc2ba48-2951-4c84-8753-04d700abeedd.png)
- confirm
  ![image](https://user-images.githubusercontent.com/118882411/224496521-f962aba0-ce6a-467f-8ec6-07ab5c440653.png)
- go to instance tab and check
  ![image](https://user-images.githubusercontent.com/118882411/224496576-01f64f9d-b65c-4da7-9b76-4e5f4e9c1e49.png)

## Next Steps

- AWS Systems Manager (SSM), AWS OpsWorks
