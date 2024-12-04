[//]: # (Title: Troubleshooting - Stella Mod Docs)
[//]: # (Description: )
[//]: # (Tags: )
[//]: # (Canonical: /genshin-stella-mod/docs?page=troubleshooting)
[//]: # (Contributors: Sefinek)

## ERR_CONNECTION_TIMED_OUT {#ERR_CONNECTION_TIMED_OUT}
This error is currently known to occur primarily in Brazil. The reason might be a block of certain Cloudflare IP address ranges by your Internet Service Provider (ISP).
Unfortunately, we have no direct control over this. To resolve the issue, you can:
1. Contact your ISP's support team and report the problem.
2. Use a VPN to bypass the ISP restrictions (this might affect your trust factor).

## Unhandled exception. System.NullReferenceException: Object reference not set to an instance of an object. {#NullReferenceException}
This error usually occurs in Genshin Stella Mod. Try deleting the FPS Unlocker configuration file, as it might be corrupted or empty.
```
C:\Program Files\Sefinek\Genshin-Stella-Mod\net8.0-windows10.0.22621.0\data\unlocker\unlocker.config.json
```