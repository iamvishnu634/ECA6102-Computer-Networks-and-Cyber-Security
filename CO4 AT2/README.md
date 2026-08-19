**Forensic Investigation of a Simulated Cyber Incident**



One of the critical aspects of computer forensic investigation involves determining the nature and origin of the suspicious activity in question. For this exercise, a simulated computer crime was investigated using Windows PowerShell commands. It is expected that the investigation will provide answers to some of the following questions: Are there any signs of a possible compromise in the system? What digital evidence can be extracted for use in court? What does the evidence suggest about the sequence of events and how it has led to the current situation?



**Evidence Collection and Analysis**



First, a log file that described the incident to be investigated was created for the purposes of this exercise. It contained the following information:



There were three failed attempts to log in as admin, and one successful attempt. All requests came from the same source IP address: 192.168.1.50. The failed attempts were suspicious and possibly indicated brute-force activity or an attempted privilege escalation. The simulated incident was saved as a piece of digital evidence in a separate file for further analysis with Windows PowerShell.



The analysis started with parsing the log file with Select-String command in order to locate the relevant lines of text. The timestamps helped to understand the context and establish the chronological order of the events depicted in the log.



The analysis showed three failed attempts to log in as admin before the successful attempt. It suggests that there are clues in the evidence file of a possible privilege escalation or brute-force attack that may have led to a compromise of the system. The evidence file was hashed with the Get-FileHash command to ensure data integrity and to provide a means of verifying the evidence file’s authenticity at a later date.



**Findings**



There were three failed attempts to log in as admin. The requests came from the same source IP address, 192.168.1.50. One of the attempts was successful, which resulted in establishing an admin-level session. The timestamps depicted in the log allowed to establish the chronological order of the events.



The evidence file suggests that there is a possibility of a privilege escalation or brute-force attack taking place. A SHA-256 hash value was calculated for the evidence file.



**Conclusion**



The exercise provided an opportunity to participate in a simulated forensic investigation of a computer-related crime. The incident log file was analyzed in order to extract the necessary information for further analysis. The timestamps depicted in the log allowed to ascertain the chronological order of the events. The results of the analysis demonstrated that the evidence file contains suspicious data that may suggest a number of security-related concerns.



In the case of a real-life scenario, it would be advisable to take immediate action to prevent further damage or deletion of evidence. For instance, the investigation would involve looking into the contents of the server in question, checking for signs of unauthorized access, and responding accordingly. In order to avoid similar incidents in the future, it would be recommended to implement strong passwords, configure the servers to deny multiple login attempts, and utilize additional security measures, such as Multi-Factor Authentication.



Tools used: Windows PowerShell, authentication log file, hashing, Snipping tool, GitHub.

