# Administering an AlloyDB Database || [GSP1086](https://www.cloudskillsboost.google/focuses/100851?parent=catalog) ||

### Run the following Commands in CloudShell

```
export ZONE=$(gcloud compute instances list alloydb-client --format 'csv[no-heading](zone)')

gcloud compute ssh alloydb-client --project=$DEVSHELL_PROJECT_ID --zone=$ZONE --quiet
```
```
export ALLOYDB=
```

* Go to `AlloyDB Clusters` from [here](https://console.cloud.google.com/alloydb/clusters?)

```
echo $ALLOYDB  > alloydbip.txt 
psql -h $ALLOYDB -U postgres
```

* Paste The Following Password

```
Change3Me
```
```
\c postgres
```
```
CREATE EXTENSION IF NOT EXISTS PGAUDIT;
```
```
select extname, extversion from pg_extension where extname = 'pgaudit';
```
```
\q
```
```
exit
```
```
export ZONE=$(gcloud compute instances list alloydb-client --format 'csv[no-heading](zone)')
export REGION="${ZONE%-*}"
gcloud alloydb instances create lab-instance-rp1 \
  --cluster=lab-cluster \
  --region=$REGION \
  --instance-type=READ_POOL \
  --cpu-count=2 \
  --read-pool-node-count=2
```

* Open New Cloudshell tab

```
export ZONE=$(gcloud compute instances list alloydb-client --format 'csv[no-heading](zone)')
export REGION="${ZONE%-*}"
gcloud beta alloydb backups create lab-backup --region=$REGION  --cluster=lab-cluster
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

