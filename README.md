# Orca Qualys Scan Composite Action  

### Parameters
Name | Type |   | Default | Note |
|--- | ---- |---| ------- | ---- |
`config_id` | Integer | Required* | 
`orca_api_key` | Secret | Required* | 
`orca_url` | String | *Optional* | `https://orca.sherwin.com` | 
`request_timeout` | Integer | *Optional* | `20000` | 

### Response

| Variable |  Description  |
|---|---|
`response` | Response as JSON String

Usage:

```yaml
 - uses: sherwin-williams-co/sw-orca-qualys-scan-composite-action@main
   with:
     config_id: 46
     orca_api_key: '${{ secrets.BEARER_TOKEN }}'
     # Optional
     # orca_url: 'https://orca.sherwin.com'
     # request_timeout: '20000'     
```
