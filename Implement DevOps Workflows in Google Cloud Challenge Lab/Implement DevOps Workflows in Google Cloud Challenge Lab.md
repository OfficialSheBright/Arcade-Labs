# Implement DevOps Workflows in Google Cloud: Challenge Lab || [GSP330](https://www.cloudskillsboost.google/focuses/13287?parent=catalog) ||

### 📋 **Prerequisites**  

* If you do not already have a **GitHub** account, you will need to create a [GitHub account](https://github.com/signup)

### 🔐 **Recommendations**  

* Use an existing **GitHub** account if you have one. **GitHub** is more likely to block a new account as spam.

* Configure [two-factor authentication](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication) on your **GitHub account** to reduce the chances of your account being marked as **spam**.

## 🖥️ **Steps to Execute in Cloud Shell**  

### Step 1: Download and Run Script Part 1

```
curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/main/Implement%20DevOps%20Workflows%20in%20Google%20Cloud%20Challenge%20Lab/gsp330-1.sh

sudo chmod +x gsp330-1.sh

./gsp330-1.sh
```

### 🛠️ **Cloud Build Trigger Configuration**  

#### **Production Deployment Trigger:** 

| **Property**                 | **Value**        |  
| :--------------------------: | :--------------: |  
| **Name**                     | sample-app-prod-deploy |  
| **Branch Pattern**           | ^master$       |  
| **Build Configuration File** | cloudbuild.yaml |  

#### **Development Deployment Trigger:** 

| **Property**                 | **Value**        |  
| :--------------------------: | :--------------: |  
| **Name**                     | sample-app-dev-deploy |  
| **Branch Pattern**           | ^dev$          |  
| **Build Configuration File** | cloudbuild-dev.yaml |  

### Step 2: Download and Run Script Part 2

```
curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/main/Implement%20DevOps%20Workflows%20in%20Google%20Cloud%20Challenge%20Lab/gsp330-2.sh

sudo chmod +x gsp330-2.sh

./gsp330-2.sh
```

# 🎉 Woohoo! You Did It! 🎉

Your hard work and determination paid off!
You've successfully completed the lab. **Way to go!** 🚀

### 💬 Stay Connected with Our Community!

👉 Join the conversation and never miss an update:

💚 [**𝗪𝗵𝗮𝘁𝘀𝗔𝗽𝗽 𝗖𝗼𝗺𝗺𝘂𝗻𝗶𝘁𝘆**](https://chat.whatsapp.com/FYKYrKwcwYDE2Xl08SEi7D) <br>
📢 [**Telegram Channel**](https://t.me/+e1HQkO3ao2FmMGQ1) <br>
👥 [**Discord**](https://discord.gg/VzBN22adUC)

#### [Solution Video](https://www.youtube.com/@officialSheBright)

