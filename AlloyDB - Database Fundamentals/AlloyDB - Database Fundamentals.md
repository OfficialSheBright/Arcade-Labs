# AlloyDB - Database Fundamentals || [GSP1083](https://www.cloudskillsboost.google/focuses/50122?parent=catalog) ||

### Run the following Commands in CloudShell

```
curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/main/AlloyDB%20-%20Database%20Fundamentals/gsp1083-1.sh

sudo chmod +x gsp1083-1.sh

./gsp1083-1.sh
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
CREATE TABLE regions (
    region_id bigint NOT NULL,
    region_name varchar(25)
) ;
ALTER TABLE regions ADD PRIMARY KEY (region_id);
```
```
INSERT INTO regions VALUES ( 1, 'Europe' );
INSERT INTO regions VALUES ( 2, 'Americas' );
INSERT INTO regions VALUES ( 3, 'Asia' );
INSERT INTO regions VALUES ( 4, 'Middle East and Africa' );
```
```
\q
```
```
exit
```
```
curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/main/AlloyDB%20-%20Database%20Fundamentals/gsp1083-2.sh

sudo chmod +x gsp1083-2.sh

./gsp1083-2.sh
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

