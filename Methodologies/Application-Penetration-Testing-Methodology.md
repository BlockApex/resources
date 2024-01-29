## What is penetration testing ?
Penetration testing (or pen testing) is a security exercise where a cyber-security expert attempts to find and exploit vulnerabilities in a computer system. The purpose of this simulated attack is to identify any weak spots in a system’s defenses which attackers could take advantage of.
While penetration testing is a common concept in traditional systems, it is much rarer in a distributed systems i.e blockchain domain.  In general, most blockchain projects only undergo a code review focusing on the project’s smart contracts or blockchain implementation.
However, blockchains are complex, multi-layered environments, and code reviews do not always cover all facets of a project’s attack surface (such as its web app).  A penetration test provides a better understanding of a blockchain project’s potential vulnerabilities and can reveal issues that other assessment techniques cannot

## What can pentested in the realm of blockchains ?
Blockchains are more popular versions of distributed systems since the advent of bitcoin in 2009. We have seem many infrastructures built around it. From a protocols perspective which runs on top of a blockchain can have many components like Web Apps, Mobile Apps, etc. Below we highlight a few components that should also be considered to get an overall sense of security of the underlying system.
- Bridges
- Layer 1 Infrastructures
   - Arbitrary Settlement & rebalancing services
   - Fraud Proof/Validity proof systems
   - Rollups & state channels
   - Arbitrary Relayers
   - DVTs
- Blockchains (due to exposed & sensitive endpoints)
- Cryptocurrency Wallets
- Digital Custody Solutions
- Web Apps
- Mobile Apps
- Composable components i.e libraries, etc

## Our approach to various systems
Each system comes with its own requirements in terms of security, compliance, and tolerance. The scope of the pentest is determined based on these factors and more. A penetration testing methodology is important to apply some standardization to this seemingly improvised effort.
- **Web/Mobile Application Testing (backend and front end)**: In this phase, we check your application thoroughly for the possible attack surfaces from where an attacker can hack or harm the organization(client) or users. We look for ways to penetrate the application (penetration testing) or try to exploit the weaknesses of the component used in a way that can harm (steal, manipulate) user's or organization’s data and/or  harm your reputation.
- **Server Testing:** This includes checking the servers (for example ec2 instance) for the ways to penetrate in it or if it runs any third party service(s) that can be exploited.
- **Network/Cloud Testing**: In this, we look for the misconfigurations in the cloud services (like s3 buckets, ec2 instances, lambda functions, load balancer, etc), that can lead to many severe attacks
- **API Testing**: in this our pentesting team will look for the way with which he can manipulate the functionality of the api’s and use it in a way to harm the application or the user.
- **Static Testing**: Here we analyze the code and try to find the bugs manually and by using SAST tools.

## Our Methodology
The below testing Methodology outlines how the BlockApex security team approaches a ‘black box’ unauthenticated  assessment process  in which no details are shared with the testing team. Our team approaches the whitebox and gray box testing as the same, because, in our experience, sometimes developers don't have the complete idea of the infrastructure, dependencies or components they are using or sometimes they simply forget to update the document.

- **Scoping** - Our Pentesting team communicates with your developers team to define the in scope items, so that we can tailor our pentesting methodology according to your business needs.. 

- **Reconnaissance and Information gathering** - Our Penetration testing team will use the latest tools and technique to find the security and technical details about the assets  in scope.

- **Vulnerability Analysis** - Our Penetration testing team will use their offensive security expertise and with the help of latest testing tools and manual techniques to identify the exploitable security vulnerabilities.

- **Exploitation** - Once a vulnerability is identified, our testing team will create a PoC and execute a plan to exploit that vulnerability but in a safe way which will minimize  any harm to the application.

- **Reporting** - Once Testing is completed our pen testers will document the detailed finding with the proper recommendations which will help to improve the security of the company. 

**Deliverables** -
At the end of the penetration testing , we provide our clients with a  comprehensive report and recommendations to remove the detected breaches:
 - Detail report of findings with the proper proof of concept (POC) wherever possible
 - List of all the vulnerabilities and their impact on the application and how easily these vulnerabilities can be exploited by the attacker (severity, impact and likelihood)
 - List of all the recommendations needed to fix the vulnerabilities.
 - A list of all the tools that were used during the testing

## Our Processes
- To read detailed process for Web pentesting see, [`Web Application Testing Process`](./Pentesting%20Checklist/Web-Application-Pentesting.md).

- To read detailed process for Mobile pentesting see, [`Mobiles Application Testing Process`](./Pentesting%20Checklist//Mobile-Application-Pentesting.md).

More will be added soon.

<hr />

Have any questions ? Reach out hello@blockapex.io or visit our website [https://blockapex.io](https://blockapex.io)