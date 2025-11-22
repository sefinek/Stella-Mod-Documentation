[//]: # (Title: Privacy Policy & Data Security – Stella Mod Documentation)
[//]: # (Description: Learn how Genshin Stella Mod handles data, protects user privacy, and ensures secure processing. This Privacy Policy explains technical data collection, Stella Mod Plus subscriber data, logs, GDPR rights, and API security.)
[//]: # (Tags: Privacy Policy, Stella Mod Privacy, Data Security, GDPR Compliance, Technical Data, Device ID, API Security, Honeypot System, Stella Mod Plus, User Data Protection, Secure Software, Stella Mod Documentation)
[//]: # (Canonical: /genshin-stella-mod/docs?page=privacy-policy)

# Privacy Policy and Data Security <!-- {#privacy-overview} -->
The Software is designed with full respect for User privacy. Your privacy is our priority.

## What Data Do We Collect? <!-- {#what-data-we-collect} -->

### Technical Data (collected automatically) <!-- {#technical-data} -->
The Software automatically collects and sends the following technical data to the Author's server:
1. **Device Identifier (Device ID)** – a unique hash generated based on the hardware identifiers of the computer. It is used for license verification, anonymous statistics, and abuse prevention.
2. **Hardware Identifiers** – to verify the device and prevent misuse, the following are collected:
    - CPU identifier (CPU ID),
    - motherboard identifier (Motherboard ID),
    - system disk identifier (Disk ID),
    - MAC address of the network card,
    - full computer name (Full Computer Name).
3. **Basic information** – IP address, operating system version, system region, Windows build number.
4. **Anti-fraud data** – results of virtual machine and debugger detection (to protect against abuse). This analysis takes place locally on the User's computer.

All data is **encrypted using cryptography** before being sent to the server.

### Data for Stella Mod Plus Subscribers <!-- {#plus-subscribers} -->
If the User has an active Stella Mod Plus subscription, additional data is collected:
1. **Account data** – email address, username.
2. **User avatar**:
    - when logging in via OAuth2 providers, only the **link to the avatar** provided by the provider (Discord, Google, Twitter, Twitch, Microsoft) is saved to the database; the avatar image itself is **not downloaded or stored** on the Author's server,
    - if the User uploads a **custom avatar**, the file is uploaded and stored on the Author's server.
3. **OAuth2 provider data** – if the User chooses to log in via an external service (Discord, Google, Twitter, Twitch, or Microsoft), profile information shared by these providers is collected, such as:
    - username,
    - email address.
4. **Discord integration** – if the User links their account to Discord, the API server may manage roles on the Discord server and send notifications (with the User's consent).
5. **Payment data** – the subscription token is linked to the email address used during purchase. Payments are processed by Stripe. The Author does not have access to payment details.
6. **User preferences** – selected mirror server, communication preferences (email, Discord), language, region.
7. **Communication history** – details of emails sent by the system (subject, date, read status) are stored to maintain a communication log.

### Logging IP Addresses and API Requests <!-- {#ip-logging} -->
Genshin Stella Mod servers automatically log basic information about backend requests, including:
- **API client IP address**,
- **exact request timestamp**,
- **API endpoint**,
- **HTTP client information (User-Agent only)**: `Mozilla/5.0 (compatible; StellaLauncher/X.Y.Z.W; +https://stella.sefinek.net)`,
- **server response status**.

#### Purpose of processing: <!-- {#ip-purpose} -->
This data is logged exclusively for:
- ensuring infrastructure security and stability,
- protecting against abuse and attacks (e.g., DDoS, brute-force, flooding),
- diagnosing technical issues,
- system performance analysis and anonymous technical statistics.

#### Legal basis: <!-- {#ip-legal-basis} -->
The legal basis for processing the IP address is **Article 6(1)(f) GDPR** — the Administrator's legitimate interest in ensuring the security and correct functioning of the service.

#### Retention period: <!-- {#ip-retention} -->
Log data is stored **temporarily**, usually no longer than **2 years**, unless longer retention is required due to security incidents or violation investigations.

#### Scope and access: <!-- {#ip-access} -->
Only the Author has access to the logs. The data is not shared with third parties unless required by law (e.g., upon request by law enforcement).  
All data is stored on a private server in Poland, without the use of cloud services or external VPS/dedicated servers.  
No other external entity has access to it.

### Do We Collect Personal Data? <!-- {#personal-data} -->
- **Free version**: The Software **does not collect personal data** during normal use. The Device ID alone cannot identify a specific person.  
  However, an **IP address** can be considered personal data under the GDPR, and is therefore processed only for the technical purposes described above.
- **Stella Mod Plus**: With an active subscription, the following personal data is collected:
    - email address and username,
    - profile data from OAuth2 providers (if used),
    - hardware identifiers linked to the User's account,
    - subscription token and payment data (processed via Stripe),
    - communication history and user preferences.

  This data is processed solely for license verification, subscription management, service delivery, and communication with the User.  
  During the payment process, user data (name, email) is transferred to Stripe in accordance with their privacy policy.
- **OAuth2 Providers**: If the User logs in using Discord, Google, Twitter, Twitch, or Microsoft, data is collected in accordance with each provider's privacy policy. The Author processes only the data required for authentication and account management.

The Software **does not monitor User activity** during gameplay and **does not store in-game actions**.  
The Software **does not use cookies or analytics tools** to track User behavior.

## Software Logs <!-- {#application-logs} -->
The Software may periodically ask whether the User wants to send Software Logs to the Author's server.  
This decision belongs **solely to the User** and **does not affect the functionality** of the Software.

### What Is Sent When Logs Are Submitted? <!-- {#logs-content} -->
If the User agrees to submit logs, the server will receive an encrypted and secured ZIP archive containing:
1. the Software's log files,
2. Device ID,
3. FPS Unlocker configuration,
4. ReShade.ini file,
5. dxdiag diagnostic report,
6. hardware specifications (CPU, RAM, GPU, disks, BIOS, battery),
7. network information, including both private and public IP addresses and other connection details.

### Additional Information <!-- {#logs-additional-info} -->
- Software Logs are strictly for diagnostic purposes. Their submission may help identify issues or bugs, but the decision to review them lies entirely with the Author.
- The Author is not obliged to review or analyze logs. Logs may be reviewed at the Author's discretion or whim if considered useful at a given moment. Most submitted logs are never analyzed or checked.
- Logs are not used for any other purpose. In particular, they are not used for profiling, marketing, or user behavior analysis.
- The User may request access to submitted logs or ask for their permanent deletion at any time. Once such a request is received, the logs will be fully and irreversibly removed.

## Secure Data Storage <!-- {#secure-storage} -->
All identifying data (e.g., device IDs) is stored in a **database on a private server physically located in Poland**.  
The server operates in a **home environment**, without cloud infrastructure or external data centers.  
This ensures full control over data processing and eliminates the risk of data exposure to third parties.  
**[sefinek.net](https://sefinek.net)** remains the **sole owner and administrator of the data**.  
NO data is shared with any external persons or institutions.

## API Security and Abuse Prevention <!-- {#api-security} -->
The current API version (v8) includes multiple mechanisms protecting against abuse, unauthorized access, and automated attacks.

### Honeypot Mechanism: Defense Against Threats <!-- {#honeypot-mechanism} -->
A **Honeypot** is a special mechanism used to detect and neutralize intrusion attempts.  
It simulates a vulnerable environment to detect suspicious activity, log attacks, and analyze their nature.

### Appeal Procedure for False Positives <!-- {#false-appeal-process} -->
IP addresses or behaviors incorrectly flagged as suspicious are reviewed and may be unblocked after analysis.  
If a User believes they have received an unjustified ban, they may file an appeal via the [ticket system](https://patrons.sefinek.net/tickets).

Each appeal is reviewed **manually and individually** to avoid unfair blocks.

## User Rights Under GDPR <!-- {#gdpr-rights} -->
Under **Regulation (EU) 2016/679 (GDPR)** the User has the right to:
- **access** their personal data,
- **rectify** incorrect data,
- **delete** their data ("right to be forgotten"),
- **restrict** data processing,
- **object** to data processing.

All data-related requests can be sent directly to contact@sefinek.net.

## Contact <!-- {#contact} -->
For matters related to privacy, data access, or data deletion, please contact the Author: **Sefinek** <<contact@sefinek.net>> ([https://sefinek.net](https://sefinek.net))

<br>
<i>Last updated: 21 November 2025</i>
