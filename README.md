# wazuh_email_report
```
docker run -d --name reporting-cli elwali/wazuh-opensearch-reporting-cli:1.0.0
```
``
Go to dashboard --> share -> snapshort --> copy short link -->
```
docker exec reporting-cli opensearch-reporting-cli -u "https://wazuh.codesec.in/goto/e3340d800170f13d16d9d7ee876b0e9b" -a basic -c "wazuh_user:wazuh_user" -s "siemalertmail@gmail.com" -r "naveen@codesecure.in" -e smtp --smtpusername "siemalertmail@gmail.com" --smtppassword "heloworld" --smtphost smtp.gmail.com --smtpport 587 --subject "Wazuh Security Report - CodeSecure Solutions" --note "Please find enclosed the Wazuh Security Report for your review."

```
