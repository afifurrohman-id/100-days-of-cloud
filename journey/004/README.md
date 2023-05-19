# IAM (Identity and Access Management), Global service (Udemy | Stephane Mareek)

## Introduction

AWS Identity and Access Management (IAM) is a web service that helps you securely control access to AWS resources. With IAM, you can centrally manage permissions that control which AWS resources users can access. You use IAM to control who is authenticated (signed in) and authorized (has permissions) to use resources. The journey will be like this:

- IAM: Users & Groups
- IAM: Permissions
- IAM Policies inheritance
- IAM Policies Structure
- IAM – Password Policy

## Cloud Research

#### IAM: Users & Groups<br>

• Root: account created by default, shouldn’t be used or shared.<br>
• Users: are people within your organization, and can be grouped.<br>
• Groups: only contain users, not other groups.<br>
• Users don’t have to belong to a group, and user can belong to multiple groups

#### IAM: Permissions!<br>

![iam-json](https://user-images.githubusercontent.com/118882411/211001146-3b60543a-7289-4e4f-9a8b-d9be12bd970c.jpg)

• Users or Groups can be assigned JSON documents called policies (JSON is a Javascript Object Notation)<br>
• These policies define the permissions of the users<br>
• In AWS you apply the least privilege principle: don’t give more permissions than a user needs<br>

#### IAM Policies inheritance

![How_SCP_Permissions_Work](https://user-images.githubusercontent.com/118882411/210993328-09d8362f-bf0a-49d4-a7ee-8e4617e9af66.png)

<br>

#### IAM Policies Structure<br>

![iam-json](https://user-images.githubusercontent.com/118882411/211001271-a47cc1ac-775a-435d-bde8-c6f1ef6a05e2.jpg)

##### Consists of:

• Version: policy language version, always include “2012 - 10 - 17”<br>
• Id: an identifier for the policy (optional)<br>
• Statement: one or more individual statements (required)<br>

##### Statements consists of:

• Sid: an identifier for the statement (optional)<br>
• Effect: whether the statement allows or denies access (Allow, Deny)<br>
• Principal: account/user/role to which this policy applied to<br>
• Action: list of actions this policy allows or denies<rb>
• Resource: list of resources to which the actions applied to <br>
• Condition: conditions for when this policy is in effect (optional)

#### IAM – Password Policy<br>

• Strong passwords = higher security for your account<br>
• In AWS, you can setup a password policy:

- Set a minimum password length
- Require specific character types:
  > including uppercase letters,
  > lowercase letters,
  > numbers,
  > non-alphanumeric characters

• Allow all IAM users to change their own passwords<br>
• Require users to change their password after some time (password expiration)<br>
• Prevent password re-use

## Next Steps

- IAM -> Multi Factor Authentication - MFA

