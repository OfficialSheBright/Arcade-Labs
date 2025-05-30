# Authentication, Authorization, and Identity with Vault || [GSP1005](https://www.cloudskillsboost.google/focuses/32203?parent=catalog) ||

### Run the following Commands in CloudShell

```
curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/main/Authentication%2C%20Authorization%2C%20and%20Identity%20with%20Vault/gsp1005-1.sh

sudo chmod +x gsp1005-1.sh

./gsp1005-1.sh
```
```
export VAULT_TOKEN=""
```
```
export VAULT_ADDR='http://127.0.0.1:8200'

vault status

vault kv put secret/mysql/webapp db_name="users" username="admin" password="passw0rd"

vault auth enable approle

vault policy write jenkins -<<EOF
# Read-only permission on secrets stored at 'secret/data/mysql/webapp'
path "secret/data/mysql/webapp" {
  capabilities = [ "read" ]
}
EOF

vault write auth/approle/role/jenkins token_policies="jenkins" \
    token_ttl=1h token_max_ttl=4h

vault read auth/approle/role/Jenkins

vault read auth/approle/role/jenkins/role-id

vault write -force auth/approle/role/jenkins/secret-id
```
```
vault write auth/approle/login role_id="REPLACE-ROLE-ID" secret_id="REPLACE-SECRET-ID"
```
```
export APP_TOKEN=""
```
```
curl -LO raw.githubusercontent.com/QUICK-GCP-LAB/2-Minutes-Labs-Solutions/main/Authentication%2C%20Authorization%2C%20and%20Identity%20with%20Vault/gsp1005-2.sh

sudo chmod +x gsp1005-2.sh

./gsp1005-2.sh
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

