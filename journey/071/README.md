
# Meet 11 - Easy Stack Floating Ip, Alarm

## Cloud Research

### Create Network
- Go to service catalog => network
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/e01cdaec-15c0-4eed-9a55-b5f8a86d9218)
- Create new
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/c278e606-4410-49ee-a491-7ad3e8f2d84c)
- Config like this, created
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/14ec6145-10e7-4d6a-9449-8d6d2ad9150d)


### Create Key Pair
- go to service catalog again and select ssh key pair
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/4a384a13-1000-43ca-8bf0-be448b8c9b1b)
- create key pair & give name
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/8fbd270f-0495-45f7-9077-bcd303837663)
- copy public and private key
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/593b8fc5-50ed-41d4-bd5d-42cd7a1e9e90)


### Create Instance
- service catalog => instance
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/839ae555-de33-4e5f-864c-93059b6640a3)
- create instance
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/b1dd33b7-ce55-4b6f-9e5f-46374da2098a)
- select os and vCPU => next
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/2ddd128e-0d93-46f2-843f-5785c3c59324)
- using your network and next
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/739fdc97-cb8f-44b4-a9ac-114ba4522577)
- using your ssh key pair
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/15245d63-68ab-4561-95b2-83eec8064e02)
- create instance
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/8c4a4f06-af29-44ed-ac1c-afa85e2fbf21)

### Router & Floating IP (To Connect Instance to the internet)
- select router in service catalog
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/c2511f80-19f8-45e4-90ea-54b5bef5d84e)
- select the router already exists 
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/43757bd9-ef0e-4bf6-8206-b19112dc36bd)
- connect subnet
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/84987637-ec9e-4f2e-8365-a1cc4c10b0da)
- select your subnet and connect 
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/4164e69c-4472-4fb6-a98f-ab6c88198331)
- go to floating ip and apply then allocate 
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/dde5dcae-f2e1-4be5-890f-53fe306f0de5)
- select your ip and associate to your vNIC
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/2ae6f705-405e-4dad-b245-3af2f16a3354)
- and associated 
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/5c8a47ad-5754-4339-9f6e-2e019dd7cbc8)

### Remote instance using ssh
- Open your terminal and using your ssh keypair.

create .pem file and paste your private key
```
 vim my-key.pem
```
try using ssh
```
ssh -i my-key.pem root@<your-public-ip>
```
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/ff2215de-dde1-48dc-86d1-7b718a4bca38)


### Alert Management
- select alert in service catalog 
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/62659173-7e67-4f91-a2ed-026155470bc6)

- create alert, select your vm and next
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/edc773dc-34d2-40e5-a62b-4c045359ddd5)

- Fill description, name & etc..
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/ee9f54cb-985f-4542-a718-3575be96b45e)
- click create contact info & fill your email
![image](https://github.com/afifurrohman-id/100-days-of-cloud/assets/118882411/9b43fdc9-585b-4d9b-807e-8b4ed8facc34)
- click created & done

## Next Steps

- ...
