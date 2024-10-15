![Security CoPilot Logo](https://github.com/Azure/Copilot-For-Security/blob/main/Images/ic_fluent_copilot_64_64%402x.png)
# NYDFS Cybersecurity regulation playbook

**Required plugins** : Microsoft Entra, Natural Language to KQL to Microsoft Defender XDR, Microsoft Defender XDR and Microsoft Purview

**Required Input**: Risky User UPN: <userupn>


**Description**: 2024 NYDFS Cybersecurity Regulation showing data for 500.7, 500.12, 500.14, 500.15, 500.16, 500.20 using CfS to bring cross platform data together from Entra, Purview, Defender XDR and Incident Anlaysis. https://www.schellman.com/blog/cybersecurity/nydfs-cybersecurity-regulation-comprehensive-guide?utm_campaign=Weekly%20Read&utm_source=hs_email&utm_medium=email&utm_content=320311797&_hsenc=p2ANqtz-9IQ88EZyZzvRFL07_Qf252wjTKblCkEM4MPxtfMdW9bYZs56rJsy60JRRXOCkW4awDUZtf4W8LfsvfNHSRIqvpSqW4Sw

1. list all users who have access to sensitive information
2. show me all data risks associated with user <userupn>
3. can you tell me which sensitive labels were seen by the above user activity
4. does the data risks shown above include encrypted data or not
5. for the above user accounts is MFA enabled
6. list all users who have access to sensitive information
7. which of the above user accounts have no MFA enabled
8. Give me a list of all Resolved incidents in Microsoft Defender with all details. Exclude Informational incidents
9. summarize the above incidents in a table. Break this down by Severity, # of Incidents, summary
10. what is the average by (last Upated Date - Created Date) for all the resolved incidents based on Severity. break it down by Severity. show it in hours.
11. Give us list of high severity defender alerts related in the last 6 months with malware determination
12. give us a list of impacted assets for the above alerts, Break it down by Device DNS Name, IP Address, User Account, File Name, File Path, Process ID, Process Name
13. describe the impact on the above assets
14. was any confidential data accessed
15. did the Impacted assets Entra user accounts have priviledged access or access to sensitive data
16. provide a detailed summary catered to a technical audience, highlight details about # of user accounts with access to sensitive information, MFA status on these accounts, data encryption authentication methods and sensitive labels accessed, incident response with details, average resolution time, details summarizing malware alerts, impacted assets and data risks involved
