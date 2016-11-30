# Azure.Routing
An example of how to get ARR Routing working in Azure.

Followed:
https://tomssl.com/2015/06/15/create-your-own-free-reverse-proxy-with-azure-web-apps/
https://www.iis.net/learn/extensions/url-rewrite-module/reverse-proxy-with-url-rewrite-v2-and-application-request-routing

Requires ARR and Rewrite 2 installed:

```powershell
iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))


Write-Host "Installing Web Platform Installer (webpicmd)"
choco install webpicmd --allowEmptyChecksums

Write-Host "Installing ARRv3 and UrlRewrite2 via Web Platform Installer (Take 2)"
webpicmd /Install /Products:"ARRv3_0,UrlRewrite2" /AcceptEULA
```
