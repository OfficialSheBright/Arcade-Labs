# Activity: Perform a SQL query

### Run the following Commands

```
SELECT device_id, email_client
FROM machines;

SELECT device_id, operating_system, OS_patch_date
FROM machines;

SELECT event_id, country
FROM log_in_attempts
WHERE country = 'Australia';

SELECT username, login_date, login_time
FROM log_in_attempts
OFFSET 4 LIMIT 1;

SELECT *
FROM log_in_attempts;

SELECT *
FROM log_in_attempts
ORDER BY login_date;

SELECT * 
FROM log_in_attempts
ORDER BY login_date, login_time;
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
