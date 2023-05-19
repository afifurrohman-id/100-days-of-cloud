# Easy stack feature introduction

## Introduction

- upload image
- create network
- create instance
- create SSH key pair
- create alert
- delete alert
- shut off instance

## Cloud Research

### Upload Image

- Go to service catalog -> Instance image
  ![image](https://user-images.githubusercontent.com/118882411/235874467-eee0e63a-75a8-4eb4-9ab3-018e2ea09028.png)
- Click Create image
  ![image](https://user-images.githubusercontent.com/118882411/235876100-e086bb23-cc74-40b6-8270-b2bd76a77628.png)
- Upload image, insert minimum RAM & etc.., and click create
  ![image](https://user-images.githubusercontent.com/118882411/235877192-20dbc19b-8474-4180-a382-514794d80b09.png)
- Confirm
  ![image](https://user-images.githubusercontent.com/118882411/236110618-647e4c9c-f58a-4339-b37e-68549cc89daf.png)

### Network and Subnets

- click service catalog and choose network
  ![image](https://user-images.githubusercontent.com/118882411/236159146-cfbdecb1-c530-4f42-809b-28e7b067bac4.png)

- Click create network
  ![image](https://user-images.githubusercontent.com/118882411/236160788-57f82201-9ed8-47a9-8dd3-a0d801a7ae17.png)

- in here, config like this and create network
  ![image](https://user-images.githubusercontent.com/118882411/236162476-4314425d-3d9a-44d0-84d7-5fa2093c48d3.png)

- Go to subnet and create subnet
  ![image](https://user-images.githubusercontent.com/118882411/236163091-787b4598-5b88-4162-b0a9-21e63b49f244.png)

- in advance configuration, setting like this & click create subnet
  ![image](https://user-images.githubusercontent.com/118882411/236163456-b15aafd8-7e89-4100-982d-ffc5d3e5c1ad.png)

### Create Instance

- Go to service catalog and click instance
  ![image](https://user-images.githubusercontent.com/118882411/236163908-84c35aa6-469b-4c40-8302-124a26387e33.png)

- Click create instance
  ![image](https://user-images.githubusercontent.com/118882411/236164253-5a7c92cb-8e74-48d4-9575-f557f0d00945.png)

- Select image
  ![image](https://user-images.githubusercontent.com/118882411/236164774-a1861954-0116-4cd8-88d8-5869bec15e4e.png)

- Then choose capacity
  ![image](https://user-images.githubusercontent.com/118882411/236165172-a168aeb6-54d8-45e7-be22-ec120640cf0b.png)

- Check delete with instance, insert size
  ![image](https://user-images.githubusercontent.com/118882411/236165659-d5ef615f-dc4f-4634-93ad-c810e46c8c7b.png)

- select network & subnet that we created earlier , click confirm
  ![image](https://user-images.githubusercontent.com/118882411/236166260-6e125d7d-b838-432f-8bfb-d84599f686c5.png)

- Before next first create keypair
  ![image](https://user-images.githubusercontent.com/118882411/236166978-9c284c59-9a66-4940-bddd-8ec6efae7a99.png)

- Insert name & copy your private key
  ![image](https://user-images.githubusercontent.com/118882411/236167166-90ff050b-d082-42b8-acc3-3859bdf0fbd3.png)

- Add your ssh key pair -> confirm & create instance
  ![image](https://user-images.githubusercontent.com/118882411/236168459-3eb1daa8-a2f0-42ed-8eee-7a29511d33ef.png)

- Confirm
  ![image](https://user-images.githubusercontent.com/118882411/236168804-e5fe30fe-136b-4eed-870b-073c08412cab.png)

### Create Alert

- Go to service catalog & select alert management
  ![image](https://user-images.githubusercontent.com/118882411/236169296-6149b574-2cd2-460d-965b-8c4f6fb741cf.png)

- Click Create alert
  ![image](https://user-images.githubusercontent.com/118882411/236169560-6af8e946-7e9d-430d-98a8-9ada84f62bc7.png)

- Select your instance
  ![image](https://user-images.githubusercontent.com/118882411/236170000-ec28ab3f-4ede-4feb-8254-956d64e4ea34.png)

- In here config like this
  ![image](https://user-images.githubusercontent.com/118882411/236170339-8b2d77d7-44d9-402d-8b31-9473b4f4ca5c.png)

- just click + icon and click create
  ![image](https://user-images.githubusercontent.com/118882411/236170821-d4b9f0b4-6261-4b81-8d13-c71a7b1994c4.png)

- You can change you want and click next
  ![image](https://user-images.githubusercontent.com/118882411/236171334-e16e5780-3dc8-4265-ad1e-f9c5d225acf2.png)

- Just save
  ![image](https://user-images.githubusercontent.com/118882411/236171565-d323f7e9-e9a4-4f43-acd2-8bba31648b6a.png)

- You can also delete your alert
  ![image](https://user-images.githubusercontent.com/118882411/236171793-e306c728-f456-453e-8b83-24c8d8df1192.png)

- Confirm
  ![image](https://user-images.githubusercontent.com/118882411/236171935-ca309c1e-1ca5-445c-a861-37d1ae0bc83b.png)

- If you end, you can shut off your instance
  ![image](https://user-images.githubusercontent.com/118882411/236172168-4ef98791-3d27-4bfb-807d-2a9ca5a18dde.png)

- Confirm
  ![image](https://user-images.githubusercontent.com/118882411/236173422-5380d437-12a8-46e0-843e-cc0cf471f0e1.png)

## Next Steps

- Vpc Section Part 1
