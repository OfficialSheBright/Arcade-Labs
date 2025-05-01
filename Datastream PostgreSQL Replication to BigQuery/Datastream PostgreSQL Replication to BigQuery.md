# Datastream: PostgreSQL Replication to BigQuery || [GSP1052](https://www.cloudskillsboost.google/focuses/53925?parent=catalog) ||

### Run the following Commands in CloudShell

```
export 
```
```
curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/refs/heads/main/Datastream%20PostgreSQL%20Replication%20to%20BigQuery/gsp1052-1.sh

sudo chmod +x gsp1052-1.sh

./gsp1052-1.sh
```

* When prompted for the password, paste the following.

```
pwd
```
```
CREATE SCHEMA IF NOT EXISTS test;

CREATE TABLE IF NOT EXISTS test.example_table (
id  SERIAL PRIMARY KEY,
text_col VARCHAR(50),
int_col INT,
date_col TIMESTAMP
);

ALTER TABLE test.example_table REPLICA IDENTITY DEFAULT; 

INSERT INTO test.example_table (text_col, int_col, date_col) VALUES
('hello', 0, '2020-01-01 00:00:00'),
('goodbye', 1, NULL),
('name', -987, NOW()),
('other', 2786, '2021-01-01 00:00:00');

CREATE PUBLICATION test_publication FOR ALL TABLES;
ALTER USER POSTGRES WITH REPLICATION;
SELECT PG_CREATE_LOGICAL_REPLICATION_SLOT('test_replication', 'pgoutput');
```
```
exit
```
```
curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/refs/heads/main/Datastream%20PostgreSQL%20Replication%20to%20BigQuery/gsp1052-2.sh

sudo chmod +x gsp1052-2.sh

./gsp1052-2.sh
```

* Use **postgres-cp** as the name and ID of the connection profile.

| Field | Value |
| :---: | :----: |
| Username | **postgres** |
| Password  | **pwd** |
| Database | **postgres** |

* Use **bigquery-cp** as the name and ID of the connection profile.

* Use **test-stream** as the name and ID of the stream

* Specify the replication slot name as **test_replication**

* Specify the publication name as **test_publication**

# 🎉 Woohoo! You Did It! 🎉

Your hard work and determination paid off!
You've successfully completed the lab. **Way to go!** 🚀

### 💬 Stay Connected with Our Community!

👉 Join the conversation and never miss an update:

💚 [**𝗪𝗵𝗮𝘁𝘀𝗔𝗽𝗽 𝗖𝗼𝗺𝗺𝘂𝗻𝗶𝘁𝘆**](https://chat.whatsapp.com/FYKYrKwcwYDE2Xl08SEi7D) <br>
📢 [**Telegram Channel**](https://t.me/+e1HQkO3ao2FmMGQ1) <br>
👥 [**Discord**](https://discord.gg/VzBN22adUC)

#### [Solution Video](https://www.youtube.com/@officialSheBright)

