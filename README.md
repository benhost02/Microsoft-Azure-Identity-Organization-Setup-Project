# Microsoft Azure Identity Organization Setup Project

<h2>Description</h2>
This project is a complete, step-by-step guide for setting up Microsoft Azure for an organization. It is designed for training, and real-world enterprise deployment. It covers account creation, domain integration, branding, identity &amp; access management (IAM), security, bulk user/group management, and Azure organizational hierarchy.
<br />

## 1. Create a Microsoft Azure Account

### Step 1: Prepare Requirements

- Valid email address (work or personal)
- Phone number (for verification)
- Debit/Credit card (for identity verification)

### Step 2: Sign Up for Azure

1. Visit [**https://azure.microsoft.com**](https://azure.microsoft.com/)

![azureReg.png](attachment:1e9cf55f-faa4-4b81-9929-0a1660e5225d:azureReg.png)

1. Click **Get Started with Azure**
2. Sign in with your Microsoft account or create a new one

![azureReg3.png](attachment:382e196c-7b43-4fce-9f7a-31a102f7209c:azureReg3.png)

1. Complete identity verification
2. Activate the **Azure Free Trial** (includes free credits)

![azureReg2.png](attachment:4af49516-e9cd-413f-9804-f65725a3ed5b:azureReg2.png)

![azurereg4.png](attachment:cbdbe72d-a6ac-41e4-8e3e-635f61f64bad:azurereg4.png)

![azurereg5.png](attachment:1fb65160-7bc7-4aa8-b571-47158616527c:azurereg5.png)

![azurereg6.png](attachment:0a123eb1-cd9a-4fde-80ea-eb475611187a:azurereg6.png)

![azurereg8.png](attachment:f638b882-e6e8-460f-ac26-afe31e466b21:azurereg8.png)

![azurereg9.png](attachment:29108c9f-dff7-4a12-94a9-802e6195c486:azurereg9.png)

### Step 3: Access Azure Portal

- Go to [**https://portal.azure.com**](https://portal.azure.com/)
- This is the main dashboard for managing all Azure resources

---

## 2. Buy a Domain Name from Namecheap

This section explains **step-by-step** how to purchase a domain name from Namecheap. This domain will later be integrated with Microsoft Azure.

---

### Step 1: Create or Log in to Namecheap Account

1. Visit **https://www.namecheap.com**
2. Click **Sign Up** (if new) or **Sign In**
3. Verify your email address after registration

---

### Step 2: Search for a Domain Name

1. On the Namecheap homepage, locate the search bar
2. Enter your desired domain name (e.g., `bnl.com.ng`)
3. Click **Search**

Namecheap will display:

- Available domains
- Alternative suggestions

---

### Step 3: Select a Domain

1. Click **Add to Cart** next to your chosen domain
2. Review domain pricing and availability

Optional add-ons:

- WHOIS Privacy (usually free for first year)
- Premium DNS (optional)

---

### Step 4: Review Cart and Checkout

1. Click **View Cart**
2. Confirm:
    - Domain name
    - Registration period (1–10 years)
3. Click **Confirm Order**

---

### Step 5: Complete Payment

1. Choose payment method:
    - Debit/Credit Card
    - PayPal
    - Account balance
2. Enter payment details
3. Click **Pay Now**

---

### Step 6: Verify Domain Purchase

1. After successful payment, go to **Account Dashboard**
2. Navigate to **Domain List**
3. Confirm your domain status shows **Active**

---

### Step 7: Access Domain DNS Management

1. From **Domain List**, click **Manage** next to the domain
2. Go to the **Advanced DNS** tab
3. This is where you will later:
    - Add TXT records (for Azure verification)
    - Manage A, CNAME, and MX records

## 3. Integrate a Custom Domain with Azure (Microsoft Entra ID)

### Step 1: Prepare Requirements

- Buy Domain name from hosting companies (eg. Namecheap, Godaddy, Whogohost)
- Or Use a Domain name that you already have

### Step 2: Open Microsoft Entra ID

1. In Azure Portal, search **Microsoft Entra ID**
2. Click **Manage → Custom domain names**

![domazure3.png](attachment:b3c66f71-3f6d-43ea-96a8-3083cf277935:domazure3.png)

### Step 3: Add Your Domain

1. Click **+ Add custom domain**

![domazure4.png](attachment:688f8e64-dc61-45a5-a5f8-c57b543e961e:domazure4.png)

1. Enter your domain name (e.g., `bnl.com.ng`)

![domazure5.png](attachment:cd854477-95ee-45f3-9912-44e2408eff46:domazure5.png)

1. Click **Add domain**

### Step 4: Verify Domain Ownership

1. Azure provides a **TXT record**

![domazure6.png](attachment:bead5da9-c50d-46bb-9682-0e1f44fbf31f:domazure6.png)

1. Log in to your domain registrar (e.g., Namecheap, GoDaddy or Whogohost)

![domazure.png](attachment:05702771-7737-4642-860c-8c948755f68a:domazure.png)

![domazure2.png](attachment:700097df-385e-4168-a5e0-0378b81ca3ad:domazure2.png)

1. Add the TXT record to DNS
2. Return to Azure and click **Verify**

![domazure7.png](attachment:e1c6855a-86c9-497d-906f-38ef545cb75f:domazure7.png)

![domazure8.png](attachment:e06eca66-037e-4da5-9226-6e833969121b:domazure8.png)

### Step 5: Set Domain as Primary (Optional)

- After verification, set the domain as **Primary** for user sign-ins

![domazureMakePrimary.png](attachment:fd466675-72b8-44f8-abc5-a7840e02790b:domazureMakePrimary.png)

![domazureMakePrimary2.png](attachment:d18b9476-e582-40a6-8794-40c9846d50c5:domazureMakePrimary2.png)

---

## 4. Customize Company Branding in Azure

### Step 1: Open Branding Settings

1. Go to **Microsoft Entra ID**
2. Select **Company branding**

![compbrand.png](attachment:6789793c-d517-44cc-a2dc-4ea208458e22:compbrand.png)

### Step 2: Configure Branding

![compbrand2.png](attachment:395b2d5d-0f1f-443b-8402-8eeee1d9cd96:compbrand2.png)

![compbrand3.png](attachment:f53df123-0abb-4d18-849a-8af09489b81b:compbrand3.png)

Upload:

- Company logo (light & dark versions)
- Background image
- Favicon

Customize:

- Sign-in page text
- Helpdesk contact details
- Privacy & terms URLs

![compbrand4.png](attachment:71cd276c-adf6-4269-b3d7-6f53742ffca9:compbrand4.png)

![compbrand5.png](attachment:7df96edf-5d59-4b86-a60e-c911593c8560:compbrand5.png)

![compbrand6.png](attachment:2943b5dd-55f6-40d8-9e00-33d120ba565b:compbrand6.png)

### Step 3: Save and Preview

- Save changes and test by opening a private browser window

![azureuserlogin.png](attachment:84b58442-6cc8-4c32-9608-939437652194:azureuserlogin.png)

![azureuserlogin2.png](attachment:794b979e-7398-4aff-b511-16aa40783cf9:azureuserlogin2.png)

---

## 5. Create Azure Entra ID (IAM) – Single User & Multiple Users

### A. Create a Single User

1. Go to **Microsoft Entra ID → Users**
2. Click **+ New user → Create new user**

![azureuser.png](attachment:55bacf25-5e2c-4a7c-b497-07de93d51ce9:azureuser.png)

![azureuser2.png](attachment:8e22697b-7a14-48fc-96d9-624e96ccc88b:azureuser2.png)

1. Fill in:
    - Username
    - Name
    - Password (auto or manual)
2. Assign:
    - Job role
    - Department
3. Click **Create**

![azureuser3.png](attachment:389bc240-d3e8-40f7-9d94-4ed9d95608ae:azureuser3.png)

![azureuser4.png](attachment:80154fe3-eb6c-4711-a3cf-563b0cd6d890:azureuser4.png)

![azureuser5.png](attachment:6b2e4545-4ed5-4559-b620-1b34682a7e5d:azureuser5.png)

### B. Create Multiple Users (Manual)

1. Go to **Users → + New user**
2. Repeat the process for each user

## **How to Invite an External User (Guest) in Azure / Microsoft Entra ID**

### **Overview**

Inviting an external user allows you to grant **secure access** to your Azure resources (apps, subscriptions, SharePoint, Teams, etc.) without creating a full internal account. External users are created as **Guest Users** in **Microsoft Entra ID** (formerly Azure Active Directory).

---

### **Step 1: Start External User Invitation**

---

1. Click **+ New user**
2. Select **Invite external user**

![azureuserin.png](attachment:aed7641d-322f-4e3a-9e52-9c595974e6ae:azureuserin.png)

---

### **Step 2: Enter Guest User Details**

Fill in the required fields:

- **Email address**
    
    → Enter the external user’s email (e.g. `partner@example.com`)
    
- **Display name**
    
    → Name that will appear in your directory
    
- **Message (optional)**
    
    → Add a custom invitation message
    
- **Send invite**
    
    → Keep enabled to send email automatically
    
    ![azureuserin2.png](attachment:1ddeeeed-385a-4103-b304-e962ffb98c82:azureuserin2.png)
    
    ![azureuserin3.png](attachment:9dd3d3ac-9e1c-4d7c-a831-cc315491bd37:azureuserin3.png)
    

(Optional)

- Add **Groups** if the user needs group-based access
- Assign **Roles** if required (e.g. Reader)

![azureuserin4.png](attachment:20127310-bac7-47d5-8c64-68da9c464789:azureuserin4.png)

---

### **Step 3: Review and Invite**

1. Review the entered details
2. Click **Invite**

![azureuserin5.png](attachment:2814b55b-ee2b-491e-8904-c7fdb40918bf:azureuserin5.png)

✅ The user is now added as a **Guest** in your tenant.

---

### **Step 4: Guest Accepts Invitation**

1. The external user receives an email invitation
2. They click **Accept invitation**
3. They sign in with:
    - Their existing Microsoft account
        
        **OR**
        
    - Create a new Microsoft account (if required)

---

### **Step 5: Verify Guest User Status**

1. Return to **Microsoft Entra ID → Users → All users**
2. Locate the invited user
3. Confirm:
    - **User type:** Guest
    - **Source:** External Azure AD / Microsoft account

---

### **Step 6: Assign Access (Optional but Recommended)**

### Assign Group

1. Open the guest user profile
2. Click **Groups**
3. Select **+ Add membership**
4. Choose the appropriate group

### Assign Role

1. Go to **Azure Subscription**
2. Click **Access control (IAM)**
3. Click **+ Add → Add role assignment**
4. Select a role (e.g. Reader)
5. Assign it to the guest user

---

### **Step 7: Manage or Remove Guest User**

### To Block Access

- Open user → Click **Block sign-in**

### To Delete Guest User

- Open user → Click **Delete**

---

## 6. Bulk User & Group Creation (CSV Method)

### Step 1: Prepare CSV File

Example format:

```
UserPrincipalName,DisplayName,FirstName,LastName,JobTitle,Department,Password
user1@domain.com,User One,User,One,IT Admin,IT,P@ssword123

```

![azurebulk.png](attachment:3e391cdc-f460-462c-9de7-d8666e2f8774:azurebulk.png)

### Step 2: Bulk User Upload

1. Go to **Microsoft Entra ID → Users**
2. Click **Bulk operations → Bulk create**
3. Download CSV Template and add your data 
    
    [UserCreateTemplate.csv](https://www.notion.so/2e3a409c571280748a6fd4ae6b34b67d?pvs=21)
    
4. Upload CSV file
5. Validate and submit

![azurebulk2.png](attachment:9fb88889-8017-439b-b588-1d543388ac7c:azurebulk2.png)

![azurebulk3.png](attachment:b02e51ab-2b5b-48ca-8693-e5ca6b2979f7:azurebulk3.png)

![azurebulk4.png](attachment:512cdfe5-f5b0-4433-8e50-524cd8623e0f:azurebulk4.png)

### Step 3: Create Groups

1. Go to **Microsoft Entra ID → Groups**
2. Click **+ New group**
3. Choose group type:
    - Security
    - Microsoft 365

### Step 4: Bulk Group Membership

- Use **Bulk operations** to add users to groups via CSV

### Step 5 Deleting Bulk Group

1. Click on the bulk Operations 
2. Select Bulk Delete
3. Click on download to download csv template for Bulk Delete
4. Edit the csv file and add the email address of the users you want to delete
5. upload the csv file and type “Yes” on the confirmation Text box
6. click the Submit Button

---

## 7. Create Azure IAM Security (Roles & Permissions)

### Step 1: Understand Azure RBAC

Azure uses **Role-Based Access Control (RBAC)**

Common roles:

- Owner
- Contributor
- Reader
- User Access Administrator

### Step 2: Assign Roles

1. Go to **Subscription / Resource Group**
2. Click **Access control (IAM)**
3. Select **+ Add → Role assignment**
4. Choose role
5. Assign to user or group

### Step 3: Best Practice

- Assign roles to **groups**, not individuals
- Use **least privilege principle**

---

## **How to Enable and Disable Azure Security Defaults**

### **Overview**

**Security Defaults** in **Microsoft Entra ID (Azure AD)** provide a basic security posture by enforcing:

- Multi-Factor Authentication (MFA) for all users
- MFA for administrators
- Blocking legacy authentication
- Protecting privileged accounts

Security Defaults are **recommended for small or new organizations** that do not use **Conditional Access policies**.

---

### **Important Notes (Read First)**

- You **cannot use Security Defaults and Conditional Access at the same time**
- Enabling Security Defaults will:
    - Force MFA registration for users
    - Block legacy authentication protocols
- Only **Global Administrators** can enable or disable Security Defaults

---

### **Prerequisites**

- Azure account with **Global Administrator** role
- Access to **Azure Portal**

---

### **Step-by-Step: Enable Azure Security Defaults**

### **Step 1: Sign in to Azure Portal**

1. Go to 👉 [https://portal.azure.com](https://portal.azure.com/)
2. Sign in with a **Global Administrator account**

---

### **Step 2: Open Microsoft Entra ID**

1. In the search bar, type **Microsoft Entra ID**
2. Select **Microsoft Entra ID**

---

### **Step 3: Open Properties**

1. From the left-hand menu, click **Properties**

---

### **Step 4: Open Security Defaults**

1. Scroll down to the bottom of the **Properties** page
2. Click **Manage security defaults**

---

### **Step 5: Enable Security Defaults**

1. Set **Enable security defaults** to **Yes**
2. (Optional) Provide a reason in the **Reason** field
3. Click **Save**

✅ **Security Defaults are now enabled**

---

### **What Happens After Enabling**

- All users will be prompted to register for **MFA**
- Admin accounts must use **MFA**
- Legacy authentication is blocked
- Users may be prompted to verify identity within **14 days**

---

### **Step-by-Step: Disable Azure Security Defaults**

### **Step 1: Sign in to Azure Portal**

1. Go to 👉 [https://portal.azure.com](https://portal.azure.com/)
2. Sign in with a **Global Administrator account**

---

### **Step 2: Open Microsoft Entra ID**

1. Search for **Microsoft Entra ID**
2. Select it

---

### **Step 3: Go to Properties**

1. Click **Properties** from the left menu

---

### **Step 4: Manage Security Defaults**

1. Scroll to the bottom
2. Click **Manage security defaults**

---

### **Step 5: Disable Security Defaults**

1. Set **Enable security defaults** to **No**
2. Enter a **reason** (recommended)
3. Click **Save**

❌ **Security Defaults are now disabled**

---

## **When Should You Disable Security Defaults?**

You should disable Security Defaults **only if**:

- You plan to use **Conditional Access policies**
- You need **custom MFA rules**
- You require **exceptions for service accounts**
- You are implementing **Zero Trust architecture**

---

## **Best Practices**

- Use **Security Defaults** for small environments
- Use **Conditional Access** for advanced environments
- Always enforce **MFA for administrators**
- Monitor sign-ins via **Entra ID → Sign-in logs**
- Review authentication methods regularly

---

## **Troubleshooting**

**Users not prompted for MFA?**

- Check if Conditional Access policies exist
- Confirm Security Defaults are enabled

**Legacy app stopped working?**

- Security Defaults block legacy authentication
- Replace with modern authentication

---

## **Quick Summary**

| Action | Location |
| --- | --- |
| Enable Security Defaults | Entra ID → Properties → Manage security defaults |
| Disable Security Defaults | Entra ID → Properties → Manage security defaults |
| Required Role | Global Administrator |

## 8. Create Azure IAM Security Policies

### Step 1: Conditional Access Policies

1. Go to **Microsoft Entra ID → Security → Conditional Access**
2. Click **+ New policy**

Examples:

- Require MFA for admins
- Block sign-in from risky countries
- Require compliant devices

### Step 2: Enable Multi-Factor Authentication (MFA)

1. Go to **Users → Per-user MFA**
2. Enable MFA for selected users

## **How to Enable Per-User MFA in Azure (Microsoft Entra ID)**

### **Overview**

**Per-User MFA** allows you to manually enable or enforce MFA for **specific users** instead of applying it tenant-wide. This method is considered **legacy** but is still available and useful for basic environments.

⚠️ **Note:** Microsoft recommends **Conditional Access** over Per-User MFA for modern security.

---

### **Prerequisites**

- Azure account
- **Global Administrator** or **Authentication Administrator** role
- Security Defaults must be **disabled**

---

### **Important Before You Start**

- You **cannot use Per-User MFA if Security Defaults are enabled**
- Per-User MFA is configured outside the main Entra ID blade
- MFA applies to **all sign-ins** for the selected user

---

### **Step 1: Sign in to Azure Portal**

1. Go to 👉 [https://portal.azure.com](https://portal.azure.com/)
2. Sign in with an **admin account**

---

### **Step 2: Open Microsoft Entra ID**

1. In the search bar, type **Microsoft Entra ID**
2. Click **Microsoft Entra ID**

---

### **Step 3: Open Users**

1. From the left-hand menu, click **Users**
2. Select **All users**

---

### **Step 4: Open Per-User MFA Settings**

1. At the top menu, click **Per-user MFA**
    - This opens the **Multi-Factor Authentication** portal in a new tab

---

### **Step 5: Select the User**

1. In the MFA portal, locate the user
2. Check the box next to the user’s name

---

### **Step 6: Enable MFA**

1. On the right-hand side, click **Enable**
2. Confirm by clicking **Enable multi-factor auth**

🟡 User status becomes **Enabled**

---

### **Step 7: Enforce MFA (Recommended)**

1. Select the same user again
2. Click **Enforce**
3. Confirm the action

🟢 User status changes to **Enforced**

---

### **MFA Status Explained**

| Status | Meaning |
| --- | --- |
| Disabled | MFA not enabled |
| Enabled | User registers MFA but may not be prompted immediately |
| Enforced | MFA required at every sign-in |

---

### **Step 8: User MFA Registration**

1. User signs in to 👉 https://mysignins.microsoft.com/security-info
2. User sets up:
    - Microsoft Authenticator app (recommended)
    - SMS or voice call (if allowed)

---

### **Step 9: Test MFA**

1. Ask the user to sign out
2. Sign in again at 👉 [https://portal.office.com](https://portal.office.com/)
3. MFA prompt should appear

---

### **Step-by-Step: Disable Per-User MFA**

### **Step 1: Open Per-User MFA Portal**

- Entra ID → Users → **Per-user MFA**

---

### **Step 2: Select the User**

- Check the user account

---

### **Step 3: Disable MFA**

1. Click **Disable**
2. Confirm the action

🔴 MFA is now disabled for the user

---

### **Best Practices**

- Use **Microsoft Authenticator app**
- Enforce MFA for **admin accounts**
- Avoid using SMS where possible
- Review MFA users regularly
- Migrate to **Conditional Access** when possible

---

### **Limitations of Per-User MFA**

- No app-based conditions
- No location or device filtering
- No exceptions or exclusions
- Legacy authentication may still work unless blocked

---

### **When to Use Per-User MFA**

✅ Small tenants

✅ Testing environments

❌ Large organizations

❌ Zero Trust implementations

---

### **Quick Summary**

| Task | Location |
| --- | --- |
| Enable MFA | Entra ID → Users → Per-user MFA |
| Enforce MFA | MFA portal → Enforce |
| Disable MFA | MFA portal → Disable |
| User Setup | mysignins.microsoft.com |

---

## 9. Create Azure Cloud Organizational Hierarchy

### Azure Hierarchy Structure

```
Management Group
 └── Subscription
      └── Resource Group
           └── Resources

```

### Step 1: Create Management Groups

1. Go to **Management Groups**
2. Click **+ Create**
3. Name groups based on business structure:
    - Company
    - Departments (IT, Finance, DevOps)

### Step 2: Assign Subscriptions

- Move subscriptions under appropriate management groups

### Step 3: Create Resource Groups

1. Go to **Resource groups**
2. Click **+ Create**
3. Name using standard format:
    - `rg-it-prod`
    - `rg-dev-test`

---

## 10. Recommended Naming Conventions

- Users: `firstname.lastname@domain.com`
- Groups: `GRP-AZ-IT-ADMINS`
- Resource Groups: `rg-department-env`

---

## 11. Security & Governance Best Practices

- Enable MFA for all users
- Use Privileged Identity Management (PIM)
- Audit sign-ins regularly
- Apply Azure Policies at management group level
- Log activities using Azure Monitor

---

## 12. Project Outcome

By completing this project, you will have:

- A fully configured Azure tenant
- Secure identity & access management
- Proper organizational hierarchy
- Enterprise-ready Azure environment

---

**Author:** Engr. Ukachukwu Benjamin

**Use Case:** Cloud Security, DevOps, Enterprise IAM
