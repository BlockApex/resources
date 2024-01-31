## What is penetration testing?
Penetration testing (or pen testing) is a security exercise where a cyber-security expert attempts to find and exploit vulnerabilities in a computer system. The purpose of this simulated attack is to identify any weak spots in a system’s defenses that attackers could take advantage of.
While penetration testing is a common concept in traditional systems, it is much rarer in distributed systems i.e. blockchain domain.  In general, most blockchain projects only undergo a code review focusing on the project’s smart contracts or blockchain implementation.
However, blockchains are complex, multi-layered environments, and code reviews do not always cover all facets of a project’s attack surface (such as its web app).  A penetration test provides a better understanding of a blockchain project’s potential vulnerabilities and can reveal issues that other assessment techniques cannot

## What can be pen-tested in the realm of blockchains?
Blockchains have become more popular versions of distributed systems since the advent of Bitcoin in 2009. We have seen many infrastructures built around it. From a protocol perspective which runs on top of a blockchain can have many components like Web Apps, Mobile Apps, etc. Below we highlight a few components that should also be considered to get an overall sense of security of the underlying system.
- Bridges
- Layer 1 Infrastructures
   - Arbitrary Settlement & rebalancing services
   - Fraud Proof/Validity proof systems
   - Rollups & state channels
   - Arbitrary Relayers
   - DVTs
- Blockchain Nodes (due to exposed & sensitive endpoints)
- Cryptocurrency Wallets
- Digital Custody Solutions
- Web Apps
- Mobile Apps
- Composable components i.e libraries, etc

## Our approach to various systems
Each system comes with its requirements in terms of security, compliance, and tolerance. The scope of the pentest is determined based on these factors and more. A penetration testing methodology is important to apply some standardization to this seemingly improvised effort.
- **Web/Mobile Application Testing (backend and front end)**: In this phase, we check your application thoroughly for possible attack surfaces from where an attacker can hack or harm the organization(client) or users. We look for ways to penetrate the application (penetration testing) or try to exploit the weaknesses of the component used in a way that can harm (steal, manipulate) user's or organization’s data and/or  harm your reputation.
- **Server Testing:** This includes checking the servers (for example ec2 instance) for the ways to penetrate it or if it runs any third-party service(s) that can be exploited.
- **Network/Cloud Testing**: In this, we look for the misconfigurations in the cloud services (like s3 buckets, ec2 instances, lambda functions, load balancer, etc), that can lead to many severe attacks
- **API Testing**: in this our pen-testing team will look for how he can manipulate the functionality of the APIs and use it in a way to harm the application or the user.
- **Static Testing**: Here we analyze the code and try to find the bugs manually and by using SAST tools.

## Our Methodology
The below testing Methodology outlines how the BlockApex security team approaches a ‘black box’ unauthenticated  assessment process  in which no details are shared with the testing team. Our team approaches the white box and gray box testing the same, because, in our experience, sometimes developers don't have the complete idea of the infrastructure, dependencies, or components they are using or sometimes they simply forget to update the document.

- **Scoping** - Our Pentesting team communicates with your developer's team to define the in-scope items, so that we can tailor our pentesting methodology according to your business needs.. 

- **Reconnaissance and Information gathering** - Our Penetration testing team will use the latest tools and techniques to find the security and technical details about the assets  in scope.

- **Vulnerability Analysis** - Our Penetration testing team will use their offensive security expertise and with the help of the latest testing tools and manual techniques identify the exploitable security vulnerabilities.

- **Exploitation** - Once a vulnerability is identified, our testing team will create a PoC and execute a plan to exploit that vulnerability but in a safe way that will minimize  any harm to the application.

- **Reporting** - Once Testing is completed our pen testers will document the detailed findings with the proper recommendations which will help to improve the security of the company. 

**Deliverables** -
At the end of the penetration testing, we provide our clients with a  comprehensive report and recommendations to remove the detected breaches:
 - A detailed report of findings with the proper proof of concepts (POCs) wherever possible.
 - A list of all the vulnerabilities and their impact on the application and how easily these vulnerabilities can be exploited by the attacker (severity, impact, and likelihood).
 - A list of all the recommendations needed to fix the vulnerabilities.
 - A list of all the tools that were used during the testing.

## Our Processes
- To read the detailed process for Web pen-testing see, [`Web Application Testing Process`](./Pentesting%20Checklist/Web-Application-Pentesting.md).

- To read the detailed process for Mobile pen-testing see, [`Mobiles Application Testing Process`](./Pentesting%20Checklist//Mobile-Application-Pentesting.md).

More will be added soon.

<hr />

Have any questions? Reach out to hello@blockapex.io or visit our website [https://blockapex.io](https://blockapex.io).
