# Meet 5 | EC2 Instance Web Server & SSH

## Cloud Research

### Create a Web Server

- GO to EC2 & Click Instance
  ![image](https://user-images.githubusercontent.com/118882411/222486623-6c26a096-8398-4249-b48b-414168927c0f.png)
- Click launch instance
  ![image](https://user-images.githubusercontent.com/118882411/222486938-5d3e625d-791e-4b54-b2c3-f9a77a31f8dc.png)
- Select os & ami
  ![image](https://user-images.githubusercontent.com/118882411/222488005-3c6cc18f-94bd-458b-b9c5-70bf8939257d.png)
- Select instance types
  ![image](https://user-images.githubusercontent.com/118882411/222488339-24eb8ebc-c505-4ae1-bbe3-357d856755dd.png)
- Create key pair (if you don't have key pair)
  ![image](https://user-images.githubusercontent.com/118882411/222488699-1aa97198-8dbd-4e15-b79e-7042ecfb1b66.png)
- Click create key pair
  ![image](https://user-images.githubusercontent.com/118882411/222489502-81474f43-2529-46f8-8b81-fbe496228fcb.png)
- Create security group (If you don't have)
  ![image](https://user-images.githubusercontent.com/118882411/222490763-ec51cf29-f86d-4baf-aaec-de7cb7d4bb3a.png)
- Add user data script (Optional) & click launch instance
  ![image](https://user-images.githubusercontent.com/118882411/222498650-2563ec0c-4fa3-4665-a271-3e8263fa05cc.png)
- Done
  ![image](https://user-images.githubusercontent.com/118882411/222491685-52b8dafa-e8fa-416b-a11a-0ead43fc084c.png)
- Comeback to instance menu and select your ec2 instance and open public DNS
  ![image](https://user-images.githubusercontent.com/118882411/222505283-0a118a73-e17c-446d-ad3a-4710b09d893b.png)
- And finally your web app is ready
  ![image](https://user-images.githubusercontent.com/118882411/222505527-0cf09cff-1184-4a72-a14b-89b82cd38723.png)

### Remote EC2 Using SSH

- Go to your key pair path & run the following command <code>ssh -i 'your-key-pair.pem' yourusername@yourippublic</code>
  ![image](https://user-images.githubusercontent.com/118882411/222494504-667684d9-862d-43e2-a9d9-8dcb015fd9de.png)

- Type "yes" and successfully to remote your EC2 Instance
  ![image](https://user-images.githubusercontent.com/118882411/222494891-668df46f-9fa3-4e69-bad4-7cc6415ca276.png)

## Next Steps

- Amazon API Gateway, Batch, Amazon Lightsail
