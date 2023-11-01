# Project : VikyGym, a local fitness and wellness center
Deploy a Static Website using Microsoft azure Virtual Machine and apply Application gateway (Load balancer ).
# Team Members : 
1)	Vivek Mane 
2)	Harshal Sonawane 
3)	Ajit Misal 

 **Case Study:** Deploying VikyGym Static Website on Azure

# Overview:

**Project Name:** VikyGym Static Website Deployment on Azure

**Client:** VikyGym, a local fitness and wellness center
# Introduction:

VikyGym, a thriving fitness and wellness center nestled in the heart of a bustling urban area, recognized the significance of extending their reach beyond their physical location. They understood that establishing an online presence was essential for reaching a wider audience and providing prospective clients with comprehensive information about their services and facilities. In collaboration with our team of Azure experts, VikyGym embarked on a transformative journey to deploy their static website on the Azure cloud platform.

## Challenges:
VikyGym faced several challenges, including:

**Lack of Online Presence:** The absence of a website limited their ability to connect with potential clients who primarily search for fitness centers and services online.

**Accessibility:** They needed to ensure that their website was accessible to users on various devices and from different locations.

**Performance:** It was crucial to optimize the website for speed and reliability to provide a seamless and engaging user experience.

**Cost Efficiency:** VikyGym needed a solution that aligned with their budget while providing scalability and reliability.

## Solution : (Services Used )

Azure VM : Azure Virtual Machines (VM): To provide enhanced functionality and dynamic content on their website, VikyGym opted for Azure VMs. These virtual machines allowed them to run specific applications and services that required server-side processing. By deploying VMs, VikyGym could execute custom code, process user data, and offer interactive features on their website, such as appointment booking, membership registration, and real-time class schedules. Azure VMs ensured flexibility, scalability, and the ability to tailor their web applications to their unique requirements.

**IIS Web Server:** We deployed Azure Virtual Machines to host the IIS (Internet Information Services) web server. This allowed us to run VikyGym's website application efficiently and provided full control over the hosting environment.

**Azure Application Gateway:** Azure Application Gateway was implemented to act as a web traffic load balancer, distributing incoming requests to the Azure VMs. This load balancing mechanism helped optimize website performance, ensuring that traffic was efficiently distributed to maintain responsiveness.

**Azure DNS (Default Azure Domain):** We used Azure DNS, including default Azure domain services, to manage domain names, configure DNS records, and route traffic to the appropriate Azure resources. This service played a vital role in ensuring that VikyGym's custom domain was correctly associated with their website hosted on Azure VMs and Application Gateway.

By combining these Azure services, we were able to create a robust and scalable infrastructure for VikyGym's website, delivering an engaging online experience for their clients and potential customers. This integrated solution ensured that the website was not only visually appealing but also highly performant and accessible, meeting VikyGym's goals of expanding their online reach and providing essential information about their services and facilities.

## Results:

This comprehensive Azure-based solution yielded the following results for VikyGym:

**Online Presence:** VikyGym successfully established a robust online presence, allowing them to connect with a wider audience and provide detailed information about their fitness and wellness services.

**Accessibility:** With Azure services, the website was accessible from various devices and locations, catering to a diverse user base.

**Performance Optimization:** Utilizing Azure VMs and load balancing with Azure Application Gateway, the website's performance was significantly improved, ensuring a smooth and responsive user experience.

**Custom Domain:** The use of Azure DNS facilitated the seamless mapping of the custom domain to the Azure VM instances, reinforcing the brand identity.

## Conclusion:

By leveraging Azure Virtual Machines, Application Gateway, and Azure DNS, VikyGym successfully overcame their challenges and achieved a compelling online presence. This solution not only met their technical requirements but also aligned with their budgetary considerations, enabling them to compete effectively in the digital space. VikyGym is now well-equipped to expand their reach, connect with potential clients, and deliver their wellness services to a broader and more diverse audience. 

# Now perform this project in the azure portal
**Sign into the Azure portal**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/547dcf70-e434-4e9f-9071-d3fda0f182e5)
**Click on Create a Resource > Virtual Machine.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/1e9b1ef2-85ec-446c-8583-dc4d3fa6d22d)
**Fill the necessary details Then select the size of the VM and give it a username and password.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/c45d465a-dff8-4503-b47a-94d5e5dcea45)
**Select the inbound ports. HTTP (80), RDP (3389) then click on ‘Next: Disks’.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/6a2c0c0d-fa9b-4fb3-af7d-dc5f6b6e31d6)
**Select the ‘standard SSD’ as OS disk type.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/ccad7259-36c8-4119-8365-8cd2e99ce677)
**Click on review and create.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/96d4f011-d89d-45bd-9495-fe8964c6903c)
**Wait for your deployment to get completed, then click on go to resource.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/772a1098-4e8d-4277-a2a9-6d1a9a207179)
**Click on the ‘Connect’ button.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/5a43a63d-3f6c-49a4-abd8-2d016fcf4966)
**In the native RDP Box click on select, then wait for it to check the prerequisites, when done download the RDP file.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/736ce398-95ba-488c-837f-bfc49b191beb)
**Now enter the Username and Password that you created and connect with remote desktop.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/10d0e925-f7e5-49c1-af56-5eaf5b8b75ff)
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/a9635a44-e3b4-4d2c-8461-cf0d0e1eacc5)
**Open the server manager dashboard > open Add Roles and Features Wizard > click on Server Roles > Web Server (IIS) and press install.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/04ca20c3-badf-49a5-8c0c-95fdfd2ff259)
**Wait for the installation to get complete**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/82aaee91-3376-422f-8900-e84e48714edf)
**Then open This PC > C: Drive > inetpub > wwwroot > .html file.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/6657dbcd-effa-4c2f-989e-2ecfbc838a75)
**Now the Delete Existing files and paste project file from our system to wwwroot folder**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/7805da30-e72c-4629-9f99-c1c94e01901c)
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/62e79f0b-5e92-4db2-b8ce-066e75dd9501)
**Copy the VM’s public IP and paste and run it through your browser.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/71704bf8-c5b6-4b2e-8e2c-b334b37f777e)
**Our Webpage is Successfully uploaded on VM**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/f2881513-3e0f-4505-bff1-54317ee748dc)
**Create One more VM  Same as previous** 
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/36da3313-332c-4a25-a77e-9d338f50137b)
**Install  Web Service (IIS)** 
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/95c7e9ab-7dcb-4527-8e8f-a4b7f79d8c2a)
**Then open This PC > C: Drive > inetpub > wwwroot > .html file. 
Now the Delete Existing files and paste project file from our system to wwwroot folder**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/60058734-9e5e-41aa-86ac-279e754198a5)
**Copy the VM 2’s public IP and paste and run it through your browser.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/e8aca275-bf25-4626-bd79-46d1bdfe26c4)
**Now deploy an application gateway (layer 7 Load Balancer) for single site. : 
Create Application gateway**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/e8acb04d-28e8-4f69-beb4-87bccf467126)
**Basic: give name > region > Tier (WAF v2) >Autoscaling (Disable) > instance count (1) > Http2 (disable) > WAF policy (create new: give name > enable bot protection).** 
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/c303d06a-1644-4d6a-b62c-e366c7b9d005)
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/3e753623-ace8-4713-8b21-eacdcd8d13f8)
**Frontend: Give name > address type (public) > ip address (create new)**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/00cdc502-8d5c-4c7e-9a1b-503baf4529b0)
**Backend: Backend pool (give name) > Target Type (add: VM1 and VM2) >add.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/d12b8d2e-4779-4f3e-85b3-ba2b8ddecdfa)
**Configuration: Routing table > give name > priority (500)> Listener> give name >
frontend_IP (public) > protocol (Http) >port (80) >Listener type (basic).**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/2cb21ffe-b5d1-4f96-b6bb-b2785b1c02b2)
**Backend target : target type (Backend pool) > backend target (backend_pool_ip) >
backend settings: give name > http > port (80) > cookie based affinity (disable) >connection
draining (disable) > add > review + create**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/91b5c81f-7566-4f50-8f98-931b4892ccc6)
**Wait for Deployment** 
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/7b37def0-c259-4d84-85a3-6e60058fae31)
**After deployment copy the Application gateway’s public ip and paste it in browser to see the load balancer work**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/813f9515-b2d2-423f-8c97-2e80f6275f83)
**Here we can see our website is loaded successfully** 
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/027440d4-f953-4e43-b432-4ae5697e54d2)
**In order to check Application gateway (Load balancer ) working properly we make some changes  in both Website Title name**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/f784b8fb-f24a-47ba-a010-dd5a82aad4f4)
**After Refreshing Tab Different Webpage loads .**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/584374cb-bb2b-4a53-8323-ec889b3c8c82)
**Here we can load balancer is working perfectly Fine.**
**Let’s Configure Default Azure DNS 
Go to Resource group >  Click on Gateway Public IP**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/9f6c88e9-be31-42cf-a29e-271f03bafaf4)
**Configuration > Give Name > save.**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/6d5f3328-43f7-41f7-b7dd-e63096d994d7)
**Copy DNS name & paste in new tab**
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/88885302-ced4-4b83-835a-33a814b6ef9b)
![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/bf997e66-5f1a-459d-a546-fff0ef4bf5b1)

# Output Of This Website :

**This is the Home page of my web site** 

![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/36ee7a7f-31cb-4c22-a862-fd47da613c2a)

**This is the About of VIKY GYM**

![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/4af393e9-844d-4f9b-90fd-449dbf308477)

**This is the CLASSIES of VIKY GYM**

![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/124305ff-867a-404a-8d6f-9721abbb2035)

**SCHEDULE Your Time for Training**  

![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/650f0484-3b22-44ae-a3be-8d704b4a4550)

**This Is The Gym Expert Trainers In Vikygym**

![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/1ce80f56-939f-44fb-83c4-52c80061fb22)

**This Is The Contact Page To Easy To Contact With Experts And join The Gym, Schedule  Your Time.**

![image](https://github.com/AJITMISAL07/AzureProject/assets/125040768/3e94f6e4-01df-42a9-a895-5545c365743b)

# Thank You









