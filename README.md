# Orca Qualys Scan Composite Action  

In order to use this action, please work with the Application Security team by visiting this [link](https://swcompany.sharepoint.com/sites/SPApplicationSecurity/SitePages/Assurance.aspx?OR=Teams-HL&CT=1642620247402&sourceId=&params=%7B%22AppName%22%3A%22Teams-Desktop%22%2C%22AppVersion%22%3A%2228%2F21110108720%22%7D#q-i-d-like-to-use-the-github-composite-action-to-kick-off-security-scans%2C-what-do-i-need-to-do-that)
to obtain required parameters specific to your needs.
### Parameters
Name | Type |   | Default | Note |
|--- | ---- |---| ------- | ---- |
`config_id` | Integer | Required* | 
`orca_api_key` | Secret | Required* | 
`orca_url` | String | *Optional* | `https://orca.sherwin.com/api/v2/task/` | 
`request_timeout` | Integer | *Optional* | `20000` | 

### Response

| Variable |  Description  |
|---|---|
`response` | Response as JSON String

Usage:

```yaml
 - uses: sherwin-williams-co/sw-orca-qualys-scan-composite-action@v2.0
   with:
     config_id: 2
     orca_api_key: '${{ secrets.API_TOKEN }}'
     # Optional
     # orca_url: 'https://orca.sherwin.com/api/v2/task/'
     # request_timeout: '20000'     
```
