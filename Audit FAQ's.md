# BlockApex Security Audit - FAQs

## Questions & Answers

### What is the time scale for an audit to complete?
The time span of an audit depends on the code size and the complexity of the project. A standard token (ERC20 & other ERC standards) can be audited within a week. However, complex DeFi projects, blockchain wallets, or dApps may take anywhere from a couple of weeks to a month.

### How many reviews will be done by the auditing team?
There will be two reviews:
1. **Initial audit**
2. **Final audit**

### Is the timeline mentioned for the Final audit?
No, the timeline mentioned applies only to the **Initial audit**. For the **Final audit**, we cannot specify a timeline as it depends on the development team. The dev team needs to fix the identified issues and provide us with the updated code before we can proceed.

### Can the BlockApex Security Team make changes in the smart contracts based on our initial review?
No, we are independent auditors and strictly follow our principles. Conducting both development and audit simultaneously would compromise the independence of the audit. However, we have development partners who can assist you: [BlockApex Labs](https://blockapex.io/labs/).

### Do we charge differently based on the programming language?
If there are no changes in the code, pricing remains the same. However, we will review both versions of the code before finalizing the pricing.

### How do we manage any modifications or new code created after the start of the audit?
We request clients to provide a **frozen GitHub commit hash** along with specifications that match the code. If a frozen commit is not provided, and major changes occur in the code during the audit, we will need to review the updated code again, which may impact the pricing and timeline.

### Apart from Smart Contract Auditing, what other services do we offer?
In addition to Smart Contract Auditing, we also offer:
- Threat Modeling
- dApps Penetration Testing
- Tokenomics Audit
- Protocol Audit
- Risk Assessment
- Fuzz-Driven Development

### Why do we conduct testing in a sandbox environment rather than public testnets?
As a leading audit company, project security is our top priority. We do not conduct functional testing on public testnets due to their inherent disadvantages, the most critical being public transaction visibility. Testing on a public testnet exposes sensitive information that malicious actors could use to devise attack strategies. 

To mitigate this risk, we fork the mainnet/testnet and perform functional tests in our own **sandbox environment**.

### What is the difference between Unit Testing and Functional Testing?
- **Unit Testing**: Conducted by developers to verify that individual smart contract features work correctly.
- **Functional Testing**: Conducted by our audit team to ensure that these features operate as intended in a real-world scenario.

### How does BlockApex minimize auditor bias?
We perform a **complete audit individually**, rather than dividing the scope among multiple auditors, to minimize auditor bias and ensure a comprehensive review.

### How does BlockApex ensure a thorough understanding of the code?
We conduct a **code walkthrough session** with the developers to understand their assumptions and gain deeper insights into the project.

### What does BlockApex provide after the Initial Audit?
After the Initial Audit, we provide a **comprehensive audit overview**, detailing our findings and security assessments.

---
For more information, visit [BlockApex](https://blockapex.io/smart-contract-audit-services/). 🚀
