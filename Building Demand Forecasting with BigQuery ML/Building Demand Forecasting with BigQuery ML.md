# Building Demand Forecasting with BigQuery ML || [GSP852](https://www.cloudskillsboost.google/focuses/16547?parent=catalog) ||

### Run the following Commands in CloudShell

```
curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/main/Building%20Demand%20Forecasting%20with%20BigQuery%20ML/gsp852-1.sh

sudo chmod +x gsp852-1.sh

./gsp852-1.sh
```

### Create the table

```
SELECT
 DATE(starttime) AS trip_date,
 start_station_id,
 COUNT(*) AS num_trips
FROM
 `bigquery-public-data.new_york_citibike.citibike_trips`
WHERE
 starttime BETWEEN DATE('2014-01-01') AND ('2016-01-01')
 AND start_station_id IN (521,435,497,293,519)
GROUP BY
 start_station_id,
 trip_date
```

* Select `SAVE RESULTS` .

* In the dropdown menu, select `BigQuery Table`.

* For Dataset select `bqmlforecast`.

* Add a Table name `training_data` .

* Click *EXPORT*.

### Run again the following Commands in CloudShell

```
curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/main/Building%20Demand%20Forecasting%20with%20BigQuery%20ML/gsp852-2.sh

sudo chmod +x gsp852-2.sh

./gsp852-2.sh
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

