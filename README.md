Update of the following table: 2026-05-05 08:28 CEST

| File | Number of malicious domains |
| ---- | ---------------- |
| full-domains-\* | 196 080 |

<details>
  <summary><b>🇫🇷 Introduction</b></summary>
  <p>

- Agrégation de listes de domaines malveillants, utilisés pour du phishing, scindée en fichiers de 131 072 entrées au maximum pour être intégrées dans des pare-feux (Fortinet **FortiGate** et autres éditeurs) ou serveurs DNS.
- Pour éviter les faux positifs, les domaines du top 1M (Cisco Umbrella et CloudFlare) des sites Web les plus visités ont été retirés.
- Domaines ordonnés en fonction du nombre de sources dans lesquelles ils apparaissent (Domaines apparaissant dans le plus de sources sont donc dans le début du fichier full-domain-aa.txt).
- Mise à jour toutes les **heures** ⏱️
- Implémentation dans les pare-feux FortiGate : [lien](https://docs.fortinet.com/document/fortigate/7.0.13/administration-guide/195303/domain-name-threat-feed)
   * Menu "Security Fabric → External Connectors → Create New → Threat Feeds → Domain Name"
   * Copier une URL dans la partie "Links" ci-dessous
   * Menu "Security Profiles → DNS Filter"
   * Dans un profil, activer "FortiGuard Category Based Filter"
   * Ajouter les listes dans "Remote Categories group"
   * Appliquer ensuite ce profil de sécurité dans vos "Firewall Policy" autorisant le protocole DNS en sortie (LAN > WAN)

</p>
</details>
<details>
  <summary><b>🇬🇧 Introduction</b></summary>
  <p>

- Aggregation of lists of malicious domains (phishing) that can be integrated into firewalls (Fortinet **FortiGate** and other vendors) and DNS servers.
- To avoid false positives, the top 1M domains (Cisco Umbrella and CloudFlare) of the most visited websites have been removed.
- Domains ordered according to the number of sources in which they appear (Domains appearing in the most sources are therefore at the beginning of the full-domain-aa.txt file).
- Updated every **hour** ⏱️
- Implementation in FortiGate firewalls: [link](https://docs.fortinet.com/document/fortigate/7.0.13/administration-guide/195303/domain-name-threat-feed)
   * Menu "Security Fabric → External Connectors → Create New → Threat Feeds → Domain Name"
   * Copy a URL in the "Links" section below
   * Menu "Security Profiles → DNS Filter"
   * In a profile, activate "FortiGuard Category Based Filter"
   * Add the lists to "Remote Categories group"
   * Then apply this security profile in your “Firewall Policy” authorizing the DNS protocol on output (LAN > WAN)

</p>
</details>
<details>
  <summary><b>🔗 URL of files to copy paste ⧉</b></summary>
  <p>

```
https://raw.githubusercontent.com/romainmarcoux/malicious-domains/main/full-domains-aa.txt
```
```
https://raw.githubusercontent.com/romainmarcoux/malicious-domains/main/full-domains-ab.txt
```
```
https://raw.githubusercontent.com/romainmarcoux/malicious-domains/main/full-domains-ac.txt
```

</p>
</details>
<details>
  <summary><b>Sources</b></summary>
  <p>

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

</p>
</details>
<details>
  <summary><b>Release Notes 📋</b></summary>
  <p>

- 2025-04-21: New sources: digitalside.it, drb-ra, malwarebytes.com, phishunt.io
- 2024-03-03: New sources: url.abuse.ch, alienvault-phishing-scam, alienvault-cert-pl, ut1-fr, phishing.army
- 2024-02-18: New source: phishtank.org
- 2024-01-20: Initial release with first sources: red.flag.domains, openphish.com, alienvault-banking-phishtank, alienvault-dropbox-phishtank, alienvault-googledocs-phishtank, alienvault-microsoft-phishtank, alienvault-paypal-phishtank

</p>
</details>
<details>
  <summary><b>🇫🇷 Qui suis-je ?</b></summary>
  <p>

Je suis expert freelance en cybersécurité, notamment sur les pare-feux.

Je maintiens ce projet depuis 2023 pour aider la communauté à se protéger contre les cybermenaces.

N'hésitez pas à me consulter pour vos besoins d'expertise pare-feux (audit, intégration, migration, problématiques ...) : voir contact ci-dessous.

</p>
</details>
<details>
  <summary><b>🇬🇧 Who am I?</b></summary>
  <p>

I am a freelance cybersecurity expert, particularly on firewalls.

I have been maintaining this project since 2023 to help the community protect itself against cyber threats.

Do not hesitate to consult me for your firewall expertise needs (audit, integration, migration, issues, etc.): see contact below.

</p>
</details>
<details>
  <summary><b>To support me 🫴</b></summary>
  <p>

[![BuyMeACoffee](https://raw.githubusercontent.com/romainmarcoux/romainmarcoux/main/img/buymeacoffee.png 'BuyMeACoffee')](https://buymeacoffee.com/romainmarcoux)
[![Paypal](https://www.paypalobjects.com/en_US/FR/i/btn/btn_donateCC_LG.gif 'Paypal')](https://www.paypal.com/donate/?hosted_button_id=TNPNMMBFVVL8E)

</p>
</details>
<details>
  <summary><b>🇫🇷 📬 Pour me contacter</b></summary>
  <p>

Contactez-moi via LinkedIn ([mon profil](https://linkedin.com/in/romainmarcoux/)) pour :
- m'indiquer des faux positifs
- me proposer d'ajouter une **autre** source de domaines malveillants (voir section "Sources" ci-dessus)
- me solliciter pour vos besoins d'expertise pare-feux (audit, intégration, migration, problématiques ...)
- me remercier et m'encourager pour le maintien de ce projet 😉

</p>
</details>
<details>
  <summary><b>🇬🇧 📬 To contact me</b></summary>
  <p>

Contact me via LinkedIn ([my profile](https://linkedin.com/in/romainmarcoux/)) to:
- notify me false positives
- suggest I add **another** source of malicious domains (see "Sources" section above)
- to consult me for your firewall expertise needs (audit, integration, migration, issues, etc.)
- thank me and encourage me for maintaining this project 😉

</p>
</details>

