Offensive Security Intro
<img width="1913" height="853" alt="image" src="https://github.com/user-attachments/assets/306aee37-4a41-4be3-a1ea-530865302fd4" />
📌 Room Overview
This TryHackMe room introduces the concept of Offensive Security through a simulated real-world scenario. The lab demonstrates how ethical hackers identify vulnerabilities in web applications and exploit them in a controlled and legal environment to improve system security.

🎯 Objectives
Understand the concept of Offensive Security
Learn how attackers discover hidden web directories
Perform directory brute-forcing using Gobuster
Exploit access control vulnerabilities
Simulate an unauthorized banking transaction

📍 Task 1: What is Offensive Security?
Offensive Security is the practice of actively testing computer systems by simulating the techniques used by attackers to identify security weaknesses before they can be exploited maliciously.
It involves:
Breaking into systems
Exploiting software bugs
Identifying vulnerabilities
Gaining unauthorized access (ethically)

✅ Answer:
Offensive Security

📍 Task 2: Hacking Your First Machine
A virtual machine hosting a simulated banking application named FakeBank was deployed to perform penetration testing in a safe environment.

🔎 Step 1: Directory Enumeration using Gobuster
Gobuster was used to brute-force hidden directories on the FakeBank website.
🖥️ Command Used:
gobuster -u http://fakebank.thm -w wordlist.txt dir
📤 Output:
The scan revealed the following directories:
/images (Status: 301)
/bank-transfer (Status: 200)
The /bank-transfer directory returned a 200 OK response, indicating the presence of an accessible hidden page.

💸 Step 2: Accessing the Hidden Endpoint
Navigated to the discovered endpoint:
http://fakebank.thm/bank-transfer
This page allowed users to transfer money between accounts without authentication — exposing a critical Access Control Vulnerability.

🎯 Step 3: Performing Unauthorized Transaction
An unauthorized transaction was performed:
From Account	To Account	Amount
2276	8881	$2000
Upon successful transfer, the updated balance was reflected on the account dashboard.

🏁 Result
A confirmation message was displayed indicating successful exploitation.

✅ Answer:
BANK-HACKED

🔐 Vulnerability Identified
Broken Access Control
Lack of Authentication Mechanism
Exposed Administrative Endpoint

🛠️ Tools Used
Gobuster
TryHackMe Virtual Machine
FakeBank Web Application

📚 Key Takeaways
Understood the basics of Offensive Security
Performed directory brute-forcing
Identified hidden web endpoints
Exploited a web application vulnerability
Simulated real-world banking transaction attack

🚀 Author
Riya Dhakad
Cybersecurity Enthusiast | TryHackMe Learner
