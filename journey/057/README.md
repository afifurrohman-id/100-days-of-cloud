# Meet 9 | Vpc

## Introduction

- Vpc Subnet practice

## Cloud Research

### VPC & Subnets

- Go to vpc menu
  ![image](https://user-images.githubusercontent.com/118882411/229979148-2c44a62b-2cd3-4630-9a1b-fb6ee9d87a12.png)
- Create vpc from your vpc menu
  ![image](https://user-images.githubusercontent.com/118882411/230015314-0545c538-58b0-431d-a3b3-c4809618d01d.png)
- Config like this and click create
  ![image](https://user-images.githubusercontent.com/118882411/230016022-bba51619-f233-455f-81b8-7ad832e663bb.png)
- go to subnet menu and create
  ![image](https://user-images.githubusercontent.com/118882411/230016589-cf7f2e41-19d7-47e9-94b6-86cc611e18d5.png)
- select your vpc
  ![image](https://user-images.githubusercontent.com/118882411/230016959-8a537ca7-b99f-4bca-8a86-b698b9b3d7ba.png)
- create public subnet, here the config & click create subnet
  ![image](https://user-images.githubusercontent.com/118882411/230017279-2a74888b-4ad0-47e4-8253-fd15a64c425a.png)
- create a private subnet with this config
  ![image](https://user-images.githubusercontent.com/118882411/230017921-ddf07bcd-f1cb-4b45-804e-7046b1bcb16c.png)
- confirm
  ![image](https://user-images.githubusercontent.com/118882411/230018113-f1a655a9-7689-4b70-9eb1-19e429d5cb9d.png)

### Launch instance

- First create instance in ec2 instance menu
  ![image](https://user-images.githubusercontent.com/118882411/230019014-63a83bb6-d1a3-4392-89bf-913d21f011be.png)
- create for public firstly
  ![image](https://user-images.githubusercontent.com/118882411/230019473-26bc1f06-9a7d-4ee8-a9fb-3e51b1d45824.png)
- Create new key pair
  ![image](https://user-images.githubusercontent.com/118882411/230019671-6aeaf6a2-bfea-4702-9d1f-2268f2a3c35b.png)
- Config like this
  ![image](https://user-images.githubusercontent.com/118882411/230019899-c996e984-4e96-45f0-a524-e3c09938aa13.png)
- edit network config
  ![image](https://user-images.githubusercontent.com/118882411/230020425-9e158c74-a37c-41d2-bcd2-e43b9efea286.png)
- change vpc and subnet
  ![image](https://user-images.githubusercontent.com/118882411/230020800-28ed509c-e5a4-4839-aac4-3ff8a949383b.png)
- switch to vpc menu > subnets tab and edit public vpc
  ![image](https://user-images.githubusercontent.com/118882411/230021215-3de7e4e0-19ab-4c89-9976-38dd7f9c2ede.png)
- Enable auto assign public ip & save
  ![image](https://user-images.githubusercontent.com/118882411/230021737-006944a2-c67d-4bfc-a58c-6631efb61ecb.png)
- comeback to ec2 > enable auto assign public ip
  ![image](https://user-images.githubusercontent.com/118882411/230022197-8931d634-be7b-4329-956d-56deebe101aa.png)
- Rules for ssh & click create instance
  ![image](https://user-images.githubusercontent.com/118882411/230022470-1cae93e1-f66c-4fee-a040-5834f4b72391.png)
- select your instances and click connect
  ![image](https://user-images.githubusercontent.com/118882411/230023189-d8a65e48-cac6-4300-91fb-4412dc0ab7e9.png)
- try connect and you see cannot connect to instance
  ![image](https://user-images.githubusercontent.com/118882411/230023935-227f6725-617f-446e-a2ae-066e94d2fb91.png)

### Create IGW & Route Table

- In vpc menu go to igw tab and click create
  ![image](https://user-images.githubusercontent.com/118882411/230024959-75637546-a87e-4ed5-832e-f8e0ac1c989c.png)
- fill name and create
  ![image](https://user-images.githubusercontent.com/118882411/230025177-dcc5ffe2-17be-47fd-8a70-511d162bc362.png)
- click action and attach to vpc
  ![image](https://user-images.githubusercontent.com/118882411/230025466-61ad48c0-5dcc-4e5a-b2f3-fa687fb95b32.png)
- Select vpc and attach
  ![image](https://user-images.githubusercontent.com/118882411/230025691-9ce6237e-86cb-4842-9fdd-23f48bc885f2.png)
- go to route table and create
  ![image](https://user-images.githubusercontent.com/118882411/230026059-056bd84d-af66-4a8b-b885-b6b0711ba764.png)
- first create public route table
  ![image](https://user-images.githubusercontent.com/118882411/230026361-0ae05111-8a76-41d8-92b0-51346a4c650b.png)
- private route
  ![image](https://user-images.githubusercontent.com/118882411/230026624-84766797-f01a-4155-87b6-451989e2a938.png)
- select your public route > subnet association & edit subnet association
  ![image](https://user-images.githubusercontent.com/118882411/230027035-e5c711e6-457d-4a86-a185-d37e18813b56.png)
- select public subnet & save
  ![image](https://user-images.githubusercontent.com/118882411/230027316-68924b2b-8364-45bd-ab46-839639aadeb6.png)
- do this also for private route
  ![image](https://user-images.githubusercontent.com/118882411/230027655-a3d6141e-d29d-417e-9fdb-20d6a21a3497.png)
  ![image](https://user-images.githubusercontent.com/118882411/230028025-a580293f-8254-4e95-9c74-ef2e518aa11c.png)
- edit route for public route
  ![image](https://user-images.githubusercontent.com/118882411/230028492-09272708-37bb-4eb3-86b1-39abd74ff637.png)
- add route & igw and save
  ![image](https://user-images.githubusercontent.com/118882411/230028908-b2b8b5fa-4571-4adb-9d1f-ff84117881ae.png)
- verify to connect again with your public instance
  ![image](https://user-images.githubusercontent.com/118882411/230029696-442f4d75-01a1-4e7f-961a-378679081785.png)

### Private Instance

- Go to ec2 and create instance > create new key pair
  ![image](https://user-images.githubusercontent.com/118882411/230030563-f44b93cc-4cd5-4a78-95bc-51295456c2bd.png)
- config and click create
  ![image](https://user-images.githubusercontent.com/118882411/230030958-43184d85-dcb7-4f4d-80e1-a1de968e7913.png)
- edit network setting
  ![image](https://user-images.githubusercontent.com/118882411/230031212-4065ee39-e0c1-4611-ad78-d71ea11b399d.png)
- edit sg
  ![image](https://user-images.githubusercontent.com/118882411/230033479-4547ebd4-8e9a-421b-a220-d4c22096fb12.png)
- and try connect using your public instance & you see fail
  ![image](https://user-images.githubusercontent.com/118882411/230036486-8fb61f95-bad6-459d-8547-dd7a107cf219.png)
- copy the key pair
  ![image](https://user-images.githubusercontent.com/118882411/230036843-e636d380-0570-47c3-99ad-574e3fc80686.png)
- paste and save
  ![image](https://user-images.githubusercontent.com/118882411/230037158-f4283913-ef76-4228-9010-73f796a1a959.png)
- and it's work
  ![image](https://user-images.githubusercontent.com/118882411/230038236-f0a9de0e-7969-4902-873d-22d4b8d21e6e.png)

## Next Steps

- Meet 10 | Easy Stack
