# Activity: Filter with AND, OR, and NOT

### Run the following Commands

```
SELECT *
FROM log_in_attempts
WHERE login_time > '18:00' AND success = 0;

SELECT *
FROM log_in_attempts
WHERE login_date = '2022-05-09' OR login_date = '2022-05-08';

SELECT * 
FROM log_in_attempts
WHERE NOT country LIKE 'MEX%';

SELECT * 
FROM employees
WHERE department = 'Marketing' AND office LIKE 'East-%';

SELECT * 
FROM employees
WHERE department = 'Finance' OR department = 'Sales';

SELECT * 
FROM employees
WHERE NOT department = 'Information Technology';
```

# 🎉 Woohoo! You Did It! 🎉

Your hard work and determination paid off! 💻
You've successfully completed the lab. **Way to go!** 🚀

### 💬 Stay Connected with Our Community!

👉 Join the conversation and never miss an update:

💚 [**𝗪𝗵𝗮𝘁𝘀𝗔𝗽𝗽 𝗖𝗼𝗺𝗺𝘂𝗻𝗶𝘁𝘆**](https://chat.whatsapp.com/FYKYrKwcwYDE2Xl08SEi7D) <br>
📢 [**Telegram Channel**](https://t.me/+e1HQkO3ao2FmMGQ1) <br>
👥 [**Discord**](https://discord.gg/VzBN22adUC)

#### [Solution Vedio](https://www.youtube.com/@officialSheBright)
