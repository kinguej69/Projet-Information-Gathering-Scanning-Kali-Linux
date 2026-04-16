# Projet-Information-Gathering-Scanning-Kali-Linux

🔎 Projet : Information Gathering & Scanning – Kali Linux
🎯 Objectifs
- Démontrer la maîtrise des outils Kali Linux pour la phase de reconnaissance et de scanning.
- Créer un projet reproductible et documenté pour ton portfolio GitHub.
- Illustrer un workflow complet : Reconnaissance → Scanning → Reporting.

📌 Étapes pratiques
1. Information Gathering (Reconnaissance OSINT)
- Whois / Nslookup / Dig
  
whois ecobank.com

nslookup ecobank.com

dig ecobank.com 

- theHarvester (emails, sous-domaines, hôtes)
  
theHarvester -d example.com -l 200 -b google

- Shodan (via API)
shodan search apache

- Maltego (cartographie visuelle des relations entre domaines, emails, IP).

2. Scanning Réseau
- Nmap (ports, services, OS fingerprinting)
nmap -sS -sV -O -p- example.com

- Masscan (scan rapide de grandes plages IP)
  
masscan 192.168.1.0/24 -p80,443 --rate=1000

- Nikto (scan vulnérabilités web)
  
nikto -h http://example.com

- Enum4linux (énumération SMB)
  
enum4linux -a 192.168.1.10

3. Analyse & Reporting
- Corrélation des résultats (services critiques, versions vulnérables).
- Export des résultats en XML/JSON/CSV :
nmap -sV -oX scan_results.xml example.com

✨ Valeur ajoutée
- Montre ta maîtrise des outils Kali Linux (Nmap, Masscan, Nikto, theHarvester, Enum4linux, Maltego).
- Illustre un workflow complet de pentest (reconnaissance → scanning → reporting).
- Prouve ton sens de la documentation et du partage (README clair, captures, scripts reproductibles).
- Peut être enrichi par des scénarios pratiques : détection d’un service FTP vulnérable, identification d’un sous‑domaine exposé, etc.
