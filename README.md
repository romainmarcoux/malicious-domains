# Menu:

- [Statistics](https://github.com/romainmarcoux/malicious-domains#statistics)
- [FR-EN - Introduction](https://github.com/romainmarcoux/malicious-domains#introduction)
- [Files URLs](https://github.com/romainmarcoux/malicious-domains#files-urls)
- [Sources](https://github.com/romainmarcoux/malicious-domains#sources)
- [Releases Notes](https://github.com/romainmarcoux/malicious-domains#releases-notes)
- [To support me](https://github.com/romainmarcoux/malicious-domains#to-support-me)
- [Contact](https://github.com/romainmarcoux/malicious-domains#contact)

# Statistics

Update of the following table: 2025-12-08 13:29 CEST

| File | Number of domains |
| ---- | ---------------- |
| full-domains-\* | 124 075 |

# Introduction
#### **[FR]**

- Agrégation de listes de domaines malveillants, utilisés pour du phishing, scindée en fichiers de 131 072 entrées au maximum pour être intégrées dans des pare-feux : Fortinet **FortiGate** et autres équipements.
- Pour éviter les faux positifs, les domaines du top 1M (Cisco Umbrella et CloudFlare) des sites Web les plus visités ont été retirés.
- Domaines ordonnés en fonction du nombre de sources dans lesquelles ils apparaissent (Domaines apparaissant dans le plus de sources sont donc dans le début du fichier full-domain-aa.txt).
- Mise à jour toutes les **heures**
- Implémentation dans les pare-feux FortiGate : [lien](https://docs.fortinet.com/document/fortigate/7.0.13/administration-guide/195303/domain-name-threat-feed) 
   * Menu "Security Fabric → External Connectors → Create New → Threat Feeds → Domain Name"
   * Copier une URL dans la partie "Links" ci-dessous
   * Menu "Security Profiles → DNS Filter"
   * Dans un profil, activer "FortiGuard Category Based Filter"
   * Ajouter les listes dans "Remote Categories group"
   * Appliquer ensuite ce profil de sécurité dans vos "Firewall Policy" autorisant le protocole DNS en sortie (LAN > WAN)

#### **[EN]**

- Aggregation of lists of malicious domains (phishing) that can be integrated into FortiGate firewalls and other products.
- To avoid false positives, the top 1M domains (Cisco Umbrella and CloudFlare) of the most visited websites have been removed.
- Domains ordered according to the number of sources in which they appear (Domains appearing in the most sources are therefore at the beginning of the full-domain-aa.txt file).
- Updated every **hour**
- Implementation in FortiGate firewalls: [link](https://docs.fortinet.com/document/fortigate/7.0.13/administration-guide/195303/domain-name-threat-feed)
   * Menu "Security Fabric → External Connectors → Create New → Threat Feeds → Domain Name"
   * Copy a URL in the "Links" section below
   * Menu "Security Profiles → DNS Filter"
   * In a profile, activate "FortiGuard Category Based Filter"
   * Add the lists to "Remote Categories group"
   * Then apply this security profile in your “Firewall Policy” authorizing the DNS protocol on output (LAN > WAN)

# Files URLs

```
https://raw.githubusercontent.com/romainmarcoux/malicious-domains/main/full-domains-aa.txt
https://raw.githubusercontent.com/romainmarcoux/malicious-domains/main/full-domains-ab.txt
```

# Sources

| Filename                    | Source | Description |
| --------------------------- | ------ | ----------- |
| red.flag.domains | [link](https://red.flag.domains/) | Recently registered probably malicious domain names in french TLDs |
| alienvault-banking-phishtank | [link](https://otx.alienvault.com/pulse/617b0867f77ec5e2192a4cf5) | Verified Banking Phishing Domain |
| alienvault-cert-pl | [link](https://otx.alienvault.com/pulse/653e8484ba7c285929cb5e0d) | List of malicious domains |
| alienvault-dropbox-phishtank | [link](https://otx.alienvault.com/pulse/617b082446ce0ac85e507129) | Verified Dropbox Phishing Domain |
| alienvault-googledocs-phishtank | [link](https://otx.alienvault.com/pulse/6213f2c919cb371e8d38bae5) | Verified Google Docs Phishing Domain |
| alienvault-microsoft-phishtank | [link](https://otx.alienvault.com/pulse/617b087263b19aaa7a421a2f) | Verified Microsoft Phishing Domain |
| alienvault-paypal-phishtank | [link](https://otx.alienvault.com/pulse/617b089bbbab1cd42903ced7) | Verified Paypal Phishing Domain |
| alienvault-phishing-scam | [link](https://otx.alienvault.com/pulse/5ee7247cdb3820b358b37a71) | Phishing & scam domain names |
| digitalside.it | [link](https://osint.digitalside.it/) | Malware and compromised URLs |
| drb-ra | [link](https://github.com/drb-ra/C2IntelFeeds/) | C2 Domains and URLs |
| malwarebytes.com | [link](https://www.malwarebytes.com/) | Malware and phishing Domain |
| openphish.com | [link](https://openphish.com/) | Phishing domain |
| phishing.army | [link](https://phishing.army/) | Phishing domain (only .fr domains and with main keywords) |
| phishtank.org | [link](https://phishtank.org/) | Phishing domain collaborative website |
| phishunt.io | [link](https://phishunt.io/) | Phishing domain |
| red.flag.domains | [link](https://red.flag.domains/) | Recently registered typosquatting and probably malicious domain names in french TLDs |
| url.abuse.ch | [link](https://urlhaus.abuse.ch/) | Sharing malicious domains |
| ut1-fr | [link](https://dsi.ut-capitole.fr/blacklists/) | Malware and phishing domains (only .fr domains and with main keywords) |

# Release Notes
- 2025-04-21: New sources: digitalside.it, drb-ra, malwarebytes.com, phishunt.io
- 2024-03-03: New sources: url.abuse.ch, alienvault-phishing-scam, alienvault-cert-pl, ut1-fr, phishing.army
- 2024-02-18: New source: phishtank.org
- 2024-01-20: Initial release with first sources: red.flag.domains, openphish.com, alienvault-banking-phishtank, alienvault-dropbox-phishtank, alienvault-googledocs-phishtank, alienvault-microsoft-phishtank, alienvault-paypal-phishtank

# To support me

[![BuyMeACoffee](https://raw.githubusercontent.com/romainmarcoux/romainmarcoux/main/img/buymeacoffee.png 'BuyMeACoffee')](https://buymeacoffee.com/romainmarcoux)
[![Paypal](https://www.paypalobjects.com/en_US/FR/i/btn/btn_donateCC_LG.gif 'Paypal')](https://www.paypal.com/donate/?hosted_button_id=TNPNMMBFVVL8E)

# Contact
#### **[FR]**

Contactez-moi via LinkedIn ([mon profil](https://linkedin.com/in/romainmarcoux/)) pour :
- m'indiquer des faux positifs
- être notifié quand un **nouveau segment** de fichier est créé (pour l'ajouter dans votre pare-feu)
- me proposer d'ajouter une **autre** source de domaines malveillants.

#### **[EN]**

Contact me via LinkedIn ([my profile](https://linkedin.com/in/romainmarcoux/)) to:
- notify me false positives
- be notified when a **new file** segment is created (to add it to your firewall)
- suggest I add **another** source of malicious domains.

