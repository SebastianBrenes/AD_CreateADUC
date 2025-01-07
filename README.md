<p align="center">
<img src="https://i.imgur.com/chjNHqp.png" height="50%" width="50%" alt="Active Directory Users and Computers (ADUC) logo"/>
</p>

# Creating Users and Groups (Active Directory Users and Computers - ADUC)

This guide provides a step-by-step process for creating users and groups using Active Directory Users and Computers (ADUC). Follow these instructions to effectively manage your Active Directory environment.

---

## Tools and Technologies Used

- **Platform**: Active Directory Users and Computers (ADUC)
- **Dependencies**: Active Directory Domain Services

---

## Operating Systems Used

- **Operating System**: Windows Server 2019/2022

---

## Overview of Steps

1. **Access the ADUC Console**  
   - Open the ADUC tool from the server or a remote management computer.

2. **Create a New User**  
   - Use the wizard to define user properties and attributes.

3. **Create a New Group**  
   - Set up security or distribution groups with desired scopes.

4. **Assign Users to Groups**  
   - Add users to the appropriate groups.

5. **Validate User and Group Configuration**  
   - Confirm that users and groups were created and configured correctly.

---

## Configuration Steps

### Step 1: Access the ADUC Console

- **Action**:  
  - Open the ADUC tool by navigating to **Start > Administrative Tools > Active Directory Users and Computers** or by running `dsa.msc` in the Run dialog.

<p align="center">
<img src="" height="75%" width="100%" alt="Opening ADUC console"/>
</p>

---

### Step 2: Create a New User

- **Action**:  
  - Navigate to the desired Organizational Unit (OU) in the ADUC tree.  
  - Right-click the OU, select **New > User**, and complete the wizard with the following details:  
    - **First Name**  
    - **Last Name**  
    - **User Logon Name**  
  - Set the user's password and configure account options (e.g., password reset requirements).

<p align="center">
<img src="" height="75%" width="100%" alt="Creating a new user in ADUC"/>
</p>

---

### Step 3: Create a New Group

- **Action**:  
  - Right-click the desired OU, select **New > Group**, and define the following:  
    - **Group Name**  
    - **Group Scope**: Domain Local, Global, or Universal.  
    - **Group Type**: Security or Distribution.  

<p align="center">
<img src="" height="75%" width="100%" alt="Creating a new group in ADUC"/>
</p>

---

### Step 4: Assign Users to Groups

- **Action**:  
  - Open the properties of the created group.  
  - Navigate to the **Members** tab and click **Add**.  
  - Search for and select the users to be added to the group.

<p align="center">
<img src="" height="75%" width="100%" alt="Assigning users to groups in ADUC"/>
</p>

---

### Step 5: Validate User and Group Configuration

- **Action**:  
  - Use the ADUC console to review the membership of groups and verify user attributes.  
  - Alternatively, use PowerShell commands like `Get-ADUser` and `Get-ADGroupMember` to validate configurations.

<p align="center">
<img src="" height="75%" width="100%" alt="Validating user and group configuration"/>
</p>

---

## Summary

This tutorial covered:  

- **User Creation**: Step-by-step process for creating users with required attributes.  
- **Group Creation**: Setting up security and distribution groups.  
- **User Assignment**: Adding users to appropriate groups.  
- **Validation**: Confirming proper configurations in ADUC.

By following these steps, you can efficiently manage users and groups within your Active Directory environment, ensuring proper access control and organizational structure.
