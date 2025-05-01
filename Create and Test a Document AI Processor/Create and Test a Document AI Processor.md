# Create and Test a Document AI Processor || [GSP924](https://www.cloudskillsboost.google/focuses/21028?parent=catalog) ||

### Run the following Commands in CloudShell

```
gcloud services enable documentai.googleapis.com
export ZONE=$(gcloud compute instances list document-ai-dev --format 'csv[no-heading](zone)')
gcloud compute ssh document-ai-dev --project=$DEVSHELL_PROJECT_ID --zone=$ZONE --quiet
```

* Go to `Document AI` from [here](https://console.cloud.google.com/ai/document-ai?)

* Specify the processor name as `form-parser`

* Download the [form.pdf](https://storage.googleapis.com/cloud-training/document-ai/generic/form.pdf) file to your local machine.

```
export PROCESSOR_ID=
```

```
curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/main/Create%20and%20Test%20a%20Document%20AI%20Processor/gsp924.sh

sudo chmod +x gsp924.sh

./gsp924.sh
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

