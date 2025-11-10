# NSM-IDS-Study-Lab



# 1. Purpose – What This Repository Is

This repository is a hands-on study lab documenting my deep dive into Network Security Monitoring (NSM). I’m learning how alerts are generated, how Snort behaves at the packet level, and what attacker activity actually looks like when it shows up in the logs. Everything here reflects my real, step-by-step learning process as I build the foundation of a Blue Team analyst.

I am intentionally studying NSM the “old-school way” — reading logs, inspecting traffic, writing small rules, and learning to interpret alerts without relying on heavy SIEM dashboards. This forces me to build clarity, pattern recognition, and discipline.




# 2. Background – Why I Built This

I created this lab to train myself in the fundamentals of NSM and intrusion detection. My hardware is limited, so instead of running complex dashboards or multi-node SIEMs, I’m focusing on the actual skills an analyst needs:

understanding alerts

interpreting suspicious behavior

capturing traffic

reviewing logs manually

learning how detection rules work

This repository exists to keep my learning structured, consistent, and easy to reference as I grow.




# 3. What This Repository Contains

This repo will hold:

Snort installation + configuration notes

My custom rules and rule-testing exercises

Alert logs from scans, brute force attempts, and local rule triggers

Packet inspection notes and small examples

Screenshots of Snort in action

Breakdowns of what each alert means in plain language

Weekly reflections on what I learned and what needs work

This is not a production build — it is a training ground to sharpen my analysis skills.




# 4. Example – What This Lab Looks Like in Action

```bash

Sample Snort Alert Output (Example):

[**] [1:1000001:1] ICMP Test Rule Triggered [**]
[Priority: 0] 
10/10-14:52:11.123456 192.168.1.10 -> 192.168.1.20
ICMP TTL:64 TOS:0x0 ID:54321 IpLen:20 DgmLen:84

```

Interpretation (My Learning Example):

A basic ICMP packet triggered my custom rule.

Confirms Snort configuration and rule path are correct.

Useful for validating my rule syntax before moving into more complex detections.

Screenshots, logs, and full explanations will be added throughout the repo.




# 5. Repository Structure
NSM-IDS-Study-Lab/
│
├── setup/                 # Snort installation, config files, environment notes
├── rules/                 # Custom rules, rule testing, explanations
├── alerts/                # Raw alert logs, screenshots, timestamps
├── analysis/              # Breakdown of attacks, alert meaning, packet notes
├── captures/              # Traffic captures (safe, self-generated)
└── reflections/           # Weekly lessons, challenges, next steps


This structure keeps everything organized so I can review my progress and return to concepts when needed.




# 6. Requirements & Tools Used

This lab is built on:

Ubuntu LTS VM (VirtualBox)

Snort (community edition)

tcpdump for packet inspection

Basic Kali VM for generating test traffic

Command-line workflow only (no GUI SIEM due to hardware constraints)

Setup details and commands will be located in the /setup folder.





# 7. Caveats, Limitations & Notes

This is strictly a learning environment, not a hardened deployment.

Logs and captures are safe and self-generated — no real-world malicious samples.

My system limitations mean I am studying detection manually, which actually strengthens skill-building.

This repository evolves over time as I practice more NSM, IDS, and packet-level work.





# 8. License

No license applied at this time. Content is primarily for my education and documentation purposes.
