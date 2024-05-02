---
layout: article
title: security4Life, not just business hours
mathjax: true
---

<img src="/images/security4life.png"/>

<h2 align="left">Hardware</h2>
Router: 
- Close all unnecessary ports
- Change admin credentials
- Change name of the network and use strong access password
- Segregate the network (config Guest Wifi) for lot, home visitors...
- Smart devices (loTs) only on Guest Wifi

MFA:
- Security key for MFA (e.g. Yubikey)
- 2 phone numbers (one not shared - for bank and other crap MFA authentications) - avoiding SIM swapping
- Charge/plug your phone only to your cables/adapters (avoid public or unknown)

Crypto:
- Hardware wallet (Cold Storage for crypto - e.g. Ledger)
- Exchanges (bad) and hot wallets are less secure
- Backup your keys on paper and 2 different places

Information storage:
- NAS (e.g. Synology or... RaspberryPi NAS project!)
  - Run VMs
  - Storage/Backup
  - Photo management...

<h2 align="left">Software</h2>

Email:
- GOOD security BAD privacy (Gmail, Outlook)
- GOOD privacy (ProtonMail, Tuta)

Passwords:
- Password Manager (E.g. 1 Password, Bitwarden - open source)

Cloud storage:

- Cloud storage (prefer local backup, if not use encryption - e.g. Cryptomator
- Encrypt everything! when possible (encrypt is different to password protect) - E.g. Signal...

Privacy:
- NextDNS (for more fine tunning - RadioSignal, Little Snitch...)
- VPN (E.g. NordVPN, ProtonVPN...)
- Use DuckDuckGo instead of Google
- If you have a Yubikey, use their authenticator (instead of Google, Microsoft...)

Others:
- Avoid FREE sw - if it is free, you are the product
- Use opensource sw when available
- Docker - run several LLM locally, no wifi needed (e.g. Llama)

<h2 align="left">More</h2>

- Security AND Privacy first
- Be suspicious - don't trust, verify. If it looks like shit, smells like shit and it tastes like shit, probably is
- Don't use cloud storage for sensitive information
- "Cloud" = someone else's computer
- Email compartmentalization
    - Professional, Family, Spam, Banks...
    - Fake/alias entities online (or in stores...)
    - Don't use real personal info on social networks
- If you post a photo, remove the metadata (EXIF, IPTC, XMP)
- Don't post saying you are going, or are, somewhere, post when you return...
- Don't connect to public wifi (or use at least a VPN)
- Check for leaks on personal emails (e.g. Intelx)
- Do an OSINT lookup on yourself regularly and see what info you find (public exposure)
- Harden your mobile security (security configurations)
- Regular backups of personal files in 2 drives on 2 diff. places (E.g. CarbonCopyCloner, TimeMachine...)
- Share/help security tips with friends and family



## Hardware

| Category       | Recommendations                                                                                            |
|----------------|-------------------------------------------------------------------------------------------------------------|
| Router         | - Close all unnecessary ports<br> - Change admin credentials<br> - Change name of the network and use strong access password<br> - Segregate the network (config Guest Wifi) for lot, home visitors...<br> - Smart devices (IoTs) only on Guest Wifi |
| MFA            | - Security key for MFA (e.g. Yubikey)<br> - Use 2 phone numbers (one not shared - for bank and other sensitive MFA authentications) to avoid SIM swapping<br> - Charge/plug your phone only to your cables/adapters (avoid public or unknown) |
| Crypto         | - Hardware wallet (Cold Storage for crypto - e.g. Ledger)<br> - Exchanges (bad) and hot wallets are less secure<br> - Backup your keys on paper and store in 2 different places |
| Information storage | - NAS (e.g. Synology or RaspberryPi NAS project!)<br>   - Run VMs<br>   - Storage/Backup<br>   - Photo management... |
 
## Software

| Category       | Recommendations                                                                                            |
|----------------|-------------------------------------------------------------------------------------------------------------|
| Email          | - Most email services have GOOD security but BAD privacy (e.g. Gmail, Outlook). Choose services with GOOD privacy and GOOD Security (e.g. ProtonMail, Tutanota) |
| Passwords      | - Use a Password Manager (e.g. 1Password, Bitwarden - open source)                                         |
| Cloud storage  | - Prefer local backup, if not, use encryption (e.g. Cryptomator)                                            |
| Privacy        | - Use NextDNS for more fine-tuning (alternatives: RadioSignal, Little Snitch)<br> - Use VPN (e.g. NordVPN, ProtonVPN)<br> - Use DuckDuckGo instead of Google<br> - Use Yubikey authenticator instead of Google, Microsoft... |
| Others         | - Avoid FREE software (if it is free, you are the product)<br> - Use open-source software when available<br> - Utilize Docker to run several LLM locally, no wifi needed (e.g. Llama) |

## More

| Recommendations                                                                                            |
|-------------------------------------------------------------------------------------------------------------|
| - Prioritize Security AND Privacy first<br> - Be suspicious - don't trust, verify. If it looks like, smells like, and tastes like something malicious, it probably is<br> - Avoid using cloud storage for sensitive information<br> - Remember "Cloud" = someone else's computer<br> - Practice email compartmentalization (Professional, Family, Spam, Banks...)<br> - Remove metadata (EXIF, IPTC, XMP) from photos before posting online<br> - Avoid publicly announcing travel plans until after returning<br> - Avoid connecting to public wifi without using a VPN<br> - Regularly check for leaks on personal emails (e.g. Intelx)<br> - Conduct regular OSINT lookups on yourself to assess public exposure<br> - Harden mobile security configurations<br> - Maintain regular backups of personal files on two separate drives in different locations (e.g. CarbonCopyCloner, TimeMachine...)<br> - Share and educate friends and family about security best practices |
