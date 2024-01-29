## How to prepare for an Audit ?
We have prepared an [`audit readiness checklist`](../Audit%20readiness%20checklist/) for our clients that they can refer to prepare for an audit. This is to ensure we have a clearly defined scope & objectives for the report.

## Our Audit Methodology
At [BlockApex](https://blockapex.io), we have honed our methodology over the years and settled for the following steps for the most effective and efficient code reviews. We also keep our partners/clients enageged throughout the process.

1. **Pre-Audit**:
   The project we audit initiates with a code freeze and starts with comprehensive technical documentation. This includes access to the codebase, whitepaper, architecture details, and any other relevant materials. The provided documentation offers us a clear, high-level overview of the objectives of the code, its scope, and the specifics of its implementation. Based on the complexity of the codebase, we also scheculde a kick-off meeting to understand system assumptions to avoid false-positive & deliver a quality report.

2. **Automated & dynamic Testing**:
   We employ the several security analysis tools to unearth basic issues and gain a deeper understanding of the contracts.
   For solidity we use, [Slither](https://github.com/crytic/slither), [Mythril](https://github.com/Consensys/mythril), [Surya](https://github.com/Consensys/surya), [Echidna](https://github.com/crytic/echidna) & [Foundry](https://github.com/foundry-rs/foundry). For Solana we use, [trdelnik](https://github.com/Ackee-Blockchain/trdelnik), [X-Ray](https://www.sec3.dev/x-ray) and [Rustle](https://github.com/blocksecteam/rustle) for Near. For `GO` and `RUST` based systems, we use [Semgrep](https://github.com/trailofbits/semgrep-rules) and [golangci-lint](https://github.com/golangci/golangci-lint).
    Moreover, we also assess the codebase with our internal tools that we have developed over the years.

3. **Line-By-Line Code Review**:
   A team of security experts carefully examines each line of code `independently` to avoid bias, identifying errors and vulnerabilities. While automated tests work well for identifying bugs in the code, human engineers are more capable of detecting problems with the contract logic or architecture, poor coding practices that are technically correct and pass automated tests, gas optimization opportunities, and weak points for common attacks. A lot of the bugs and vulnerabilities that actually impact a code are protocol-specific. Finding these protocol-specific bugs requires a thorough understanding of protocol and some creativity. Any questions arised during the audit is directly relayed to the client and reponse is incorporated in the audit.
   After the review has been completed, an internal consensus meeting is held to traiage the findings & generate POCs for impacting issues.

4. **Initial Report**:
   An initial draft is produced that includes the static analysis report along with all of the findings with details outlining the issues & their remidiation. This is then sent to the client to implement fixes & get developer feedback on issues. Another review performed to ensure no additional bugs have been intorduced.

5. **Publish Final Audit Report**
   After the fixes have been thoroughly reviewed by the auditors. The final report is handed over & made publically available.

<hr />

Check out our publically available [audit reports](https://github.com/BlockApex/Audit-Reports). <br />
Have any Questions or need an audit ? Reach out at hello@blockapex.io or fill out our [form](https://blockapex.io/connect/).