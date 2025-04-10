# Windows and iSO Device Configuration and Compliance Policies

## Introduction

Multi-Factor Authentication (MFA) is being used to enhance the security of both Windows and iOS devices within the organization. By requiring users to provide two or more verification factors.

## Device Compliance Policies:

**Windows device**

**Enable BitLocker encryption**
To do that:

- I went to **Microsoft Admin page** https://admin.microsoft.com/?login#/homepage

- Sign in my Microsoft Admin Security ID.

- **Microsoft intune**

- Navigate to **Device** > **Windows** > **Compliance** 

- Create policy name. In this case, I used **Requrie bitlocker encryption**

- **Compliance setting** > **Device Health**

- Enable Required Bitlocker >> Enable Secure Boot is enabled >>  Enable Code integrity.

  <img width="958" alt="1" src="https://github.com/user-attachments/assets/883b1b0e-2c43-4d17-9e59-3cad60a890bb" />

  **Specify minimum and maximum OS versions**

  **Minimum and Maximum OS versions**

- **Compliance setting** > **Device Properties**

- Set Minimum OS versions Windows 10 22H2 (Build 19045.5608)

- Set Maximum OS versions Windows 11 24H2 (Build 26100.3476)

- <img width="1020" alt="2" src="https://github.com/user-attachments/assets/d991d78d-adcd-4404-ba3c-575e32f37e45" />

**iSO device**

**Enable Device passcode**

- I went to **Microsoft Admin page** https://admin.microsoft.com/?login#/homepage

- Sign in my Microsoft Admin Security ID.

- **Microsoft intune**

- Navigate to **Device** > **iSO** > **Compliance**

- Create policy name. In this case, I used **Enforce device passcode**

- **Compliance setting** > **System Security**

- Enable Device passcode

- <img width="955" alt="ISO A" src="https://github.com/user-attachments/assets/1ad63c9d-93da-4ff9-b94c-987312aefe02" />

- **Compliance setting** > **Microsoft Defender for Endpoint**

- Require encryption.

- <img width="956" alt="IOS B" src="https://github.com/user-attachments/assets/4d2c1974-cfab-4ef3-a358-fa3c3872b90a" />

 **Specify minimum and maximum OS versions**

  **Minimum and Maximum OS versions**

  - **Compliance setting** > **Device Properties**

  - Set Minimum OS versions iSO (16.1.1)

  - Set Maximum OS versions iSO (18.1.1)

  - ## Device Configuration Policies:

  - **Windows Devices**

  - I went to **Microsoft Admin page** https://admin.microsoft.com/?login#/homepage

  - Sign in my Microsoft Admin Security ID.

  - **Microsoft intune**

  - **(Windows Update setting)**

  - Navigate to **Device** > **Windows** > **Configuration**

  - Create policy name. In this case, I used **Windows profile**

  - Configuration setting > Windows update for business

  - <img width="958" alt="ISO C" src="https://github.com/user-attachments/assets/0d4eaccc-38ab-4a5f-81da-80818e8a765f" />

  - **(Set up Windows Defender Antivirus)**.

  - Navigate to **Device** > **Windows** > **Configuration**

  - Create policy name. In this case, I used **Windows profile**

  - **Configuration setting** > **Defender**

  - Allow Cloud Protection & Allowed Turns on Cloud Protection.

  - <img width="953" alt="ISO D" src="https://github.com/user-attachments/assets/f68f5e19-4ee1-4fc6-9e6d-d3e47cf2dad6" />

    ## Device Configuration Policies:

  - **iSO Devices**

  - (Configure email profiles)

  - <img width="959" alt="ISO E" src="https://github.com/user-attachments/assets/7c19293c-72e7-46bd-a685-a8ab5446f896" />

  ## Microsoft Defender for Endpoint Implementations.

  **Windows Devices**

   - I went to **Microsoft Admin page** https://admin.microsoft.com/?login#/homepage

   - Sign in my Microsoft Admin Security ID.

   - **Microsoft intune**

   - Navigate to **Endpoint security** > **Manage** > **Anti-virus**

   - Create policy name. In this case, I used **Denis Enable real time protection**

   - Enable real Ptotection and Network protection

   - <img width="953" alt="ISO F" src="https://github.com/user-attachments/assets/d602ff98-e96f-4aa1-9b9b-162fe8be2ffd" />

   -  **Set up attack surface reduction rules**.

   - Navigate to **Endpoint security** > **Manage** > **Attack surface reduction rules**

   - <img width="953" alt="ISO G" src="https://github.com/user-attachments/assets/b47cbae4-5d54-4f4c-8595-972fc137aa20" />

   - **Enable endpoint detection and response (EDR).**.

   - Navigate to **Endpoint security** > **Manage** > **Enable endpoint detection and response (EDR)**

   - <img width="647" alt="ISO H" src="https://github.com/user-attachments/assets/9d4e179d-ec3b-4815-8396-bdbcefc6dd9e" />

   - **iSO Device**

   - I went to **Microsoft Admin page** https://admin.microsoft.com/?login#/homepage

   - Sign in my Microsoft Admin Security ID.

   - **Microsoft intune**

   - Navigate to **Device** > **iSO** > **Compliance**

   - Create policy name. In this case, I used **Enforce device passcode**

   - **Compliance setting** > **Device Properties**

   - Set up jailbreak detection.

   - <img width="952" alt="ISO 9" src="https://github.com/user-attachments/assets/e52be5dd-a516-41df-ac1e-000020f1aec9" />

   - Navigate to **Endpoint security** > **Manage** > **conditional access policies**.

   - Create policy name. In this case, I used **Denis conditional access policies**
     
   - Enable conditional access policies

   - <img width="658" alt="ISO I" src="https://github.com/user-attachments/assets/a1b3d362-3d37-4861-997b-463b3f1652ef" />

     **Benefit for the Policy**

   - Data Protection: BitLocker encryption and device encryption for iOS ensure that data on devices is protected, even if the device is lost or stole

   - Compliance Enforcement: Ensuring devices meet compliance policies (e.g., Secure Boot, code integrity) helps maintain a secure environment

   - Centralized Management: Microsoft Intune allows for centralized management of both Windows and iOS devices, making it easier to deploy and enforce policies across the organization.

   - Multi-Factor Authentication (MFA): Implementing MFA ensures that only authenticated and authorized users can access corporate resources, adding an extra layer of security.

   - **Potential Risk**

   - Complexity and Management Overhead: Managing a comprehensive suite like Microsoft 365 E5 can be complex and may require dedicated IT resources to ensure proper configuration and maintenance.

   - Learning Curve: IT staff and end-users may require training to effectively use and manage the advanced features of Microsoft 365 E5.

   - Vulnerabilities: Incorrectly configured security settings can lead to vulnerabilities. It's crucial to follow best practices and regularly review security configurations.

   - **Recommendations for Successful Implementation**

   - Training and Awareness: Training needs to be provide for IT staff and end-users to ensure they understand the new policies and how to comply with them.

   - Regular Audits and Reviews: Regular audits and reviews of the security policies and configurations  is essentail to ensure the Polices remain effective and up-to-date.

**Conclusion** Implementing Microsoft 365 E5 licenses, along with comprehensive device management and security policies using Microsoft Intune and Microsoft Defender for Endpoint, offers significant benefits for Contoso. These benefits include enhanced security, improved device management, operational efficiency, and user productivity. By adopting a Zero Trust strategy with Multi-Factor Authentication (MFA), Contoso can ensure that only compliant endpoints access Microsoft 365 applications, further strengthening their security posture.


      
