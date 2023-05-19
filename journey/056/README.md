# Meet 8 | S3 Bucket & Static Website

## Cloud Research

### Amazon S3 - Buckets Basic

- Go to s3 Bucket menu and create a bucket
  ![image](https://user-images.githubusercontent.com/118882411/227725679-d95471b7-957a-4680-b16f-f905b02c5db9.png)
- Insert a unique bucket name & Choose your aws region after that Click create bucket -![image](https://user-images.githubusercontent.com/118882411/227725773-f106d2e4-09dc-4fff-be74-a8997902fa62.png)
- Click your bucket
  ![image](https://user-images.githubusercontent.com/118882411/227726628-af51563b-0a14-4e84-a5eb-115d1d53ac80.png)
- Go to properties tab and edit versioning
  ![image](https://user-images.githubusercontent.com/118882411/227726714-86a0e9d9-be45-4e31-89cf-99114c26e98e.png)
- Select Enable & Save changes
  ![image](https://user-images.githubusercontent.com/118882411/227726826-2b7942e0-1a53-4842-9b57-8049c57ed6e8.png)

### Amazon S3 - Static Web Hosting

- Go to end of properties menu and edit static web hosting
  ![image](https://user-images.githubusercontent.com/118882411/227726965-042ace55-9097-45f7-bf91-f09e6c5997e5.png)
- Enable Static web hosting & Save changes
  ![image](https://user-images.githubusercontent.com/118882411/227727020-466b6bc5-9efb-4dc0-9f2e-17e54a54c4d3.png)
- Go to permission menu and edit block public access
  ![image](https://user-images.githubusercontent.com/118882411/227727140-da14389c-c770-467f-bb67-98ec69d5143b.png)
- Uncheck block all public access and Save changes
  ![image](https://user-images.githubusercontent.com/118882411/227727154-6cf3b603-6ac6-4a5e-9873-6680099db894.png)
- confirm
  ![image](https://user-images.githubusercontent.com/118882411/227727194-f68f5762-6277-4b04-b3f8-019d5ef71152.png)
- Back to permission menu and Edit the bucket policy
  ![image](https://user-images.githubusercontent.com/118882411/227727298-0b8468ed-dbfe-4c42-9148-9b0998f2a0ae.png)
- Select policy generator
  ![image](https://user-images.githubusercontent.com/118882411/227727346-f306f470-4aa4-4ec5-b16d-0de9f333cd8d.png)
- Select type, insert principal to <b>\*</b> Select action to getObject
  ![image](https://user-images.githubusercontent.com/118882411/227727842-ad544ae3-940a-4483-81ea-784c7edadc36.png)
- Back to your bucket policy and copy your ARN
  ![image](https://user-images.githubusercontent.com/118882411/227727892-eecb1c47-ff46-4f8a-a8d6-e9c3de71ec2d.png)
- Back to aws policy generator, Paste your ARN, **Add /\* in the end of your ARN** and Click Add statement
  ![image](https://user-images.githubusercontent.com/118882411/227728546-bbf7abb2-1a7a-4e1f-9de7-cb3448db5188.png)
- click generate policy
  ![image](https://user-images.githubusercontent.com/118882411/227728100-b9dc8839-338d-4164-8d96-601576e7d75b.png)
- Copy JSON code
  ![image](https://user-images.githubusercontent.com/118882411/227728678-d40b303f-d80c-4a5f-99df-0b708e35640a.png)
- Back to bucket policy, paste it & Save changes
  ![image](https://user-images.githubusercontent.com/118882411/227728741-38800edc-feef-4091-83e0-fb608ea26a80.png)
- Go to Object menu and upload all file for your website
  ![image](https://user-images.githubusercontent.com/118882411/227728860-252e4072-7314-4b32-b6ba-1aae3d28c69b.png)
- Click Add File
  ![image](https://user-images.githubusercontent.com/118882411/227728894-e8560bdc-d74e-4da2-8997-367f2c3033ef.png)
- Click Upload
  ![image](https://user-images.githubusercontent.com/118882411/227729366-058546c1-3149-43e6-80a3-5dd85a1b9772.png)
- Confirm
  ![image](https://user-images.githubusercontent.com/118882411/227729439-73e2cae7-91c4-44d6-b56a-eaedcd212d4d.png)
- go to properties menu and try access your url
  ![image](https://user-images.githubusercontent.com/118882411/227729566-7fb22377-afd2-4b76-94b8-6aa326993438.png)
- And Finish
  ![image](https://user-images.githubusercontent.com/118882411/227729766-9154ce4e-3c5b-4228-be67-3e5489b54a09.png)

## Next Steps

- Meet 9 | VPC
