# Assessing Data Quality with Dataplex || [GSP1158](https://www.cloudskillsboost.google/focuses/67211?parent=catalog) ||

### Run the following Commands in CloudShell

```
export REGION=
```
```
curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/main/Assessing%20Data%20Quality%20with%20Dataplex/gsp1158.sh

sudo chmod +x gsp1158.sh

./gsp1158.sh
```

* Go to `BigQuery` from [here](https://console.cloud.google.com/bigquery?)

* In the SQL Editor, click on `Compose a new query`. Paste the following query, and then click `Run`: ( REPLACE PROJECT_ID WITH YOUR PROJECT )

```
  SELECT * FROM `PROJECT_ID.customers.contact_info`
  ORDER BY id
  LIMIT 50
```

# 🎉 Woohoo! You Did It! 🎉

Your hard work and determination paid off!
You've successfully completed the lab. **Way to go!** 🚀

### 💬 Stay Connected with Our Community!

👉 Join the conversation and never miss an update:

💚 [**𝗪𝗵𝗮𝘁𝘀𝗔𝗽𝗽 𝗖𝗼𝗺𝗺𝘂𝗻𝗶𝘁𝘆**](https://chat.whatsapp.com/FYKYrKwcwYDE2Xl08SEi7D) <br>
📢 [**Telegram Channel**](https://t.me/+e1HQkO3ao2FmMGQ1) <br>
👥 [**Discord**](https://discord.gg/VzBN22adUC)

#### [Solution Vedio](https://www.youtube.com/@officialSheBright)

#### Don't Forget to Join the [Telegram Channel](https://t.me/quickgcplab) & [Discussion group](https://t.me/quickgcplabchats)

# [QUICK GCP LAB](https://www.youtube.com/@quickgcplab)
