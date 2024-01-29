## Scope Identification
1. Share the repository url of the project's public/private `repository`.
2. Share all relavent `documentation` i.e whitepapers, websites, architecture diagrams, online docs & video tutorials (if applicable).
3. What `framework` was used to build the contracts ? i.e `Hardhat`, `Foundry`, `Truffle`, etc
4. How many `contracts` are there in the scope ?
5. What is the total `SLOC` for all of the contracts in scope ?
6. How many `libraries` does the project depends on i.e `openzeppelin`, `solday`, `layerzero`, etc.
7. How many `external calls` are there ?
8. What percentenage of `user stories` are covered in tests ?
9.  What is the overall line `coverage percentage` provided by your tests?
10. Do you expect `ERC721`, `ERC777`, `FEE-ON-TRANSFER`, `REBASING` or any other non-standard ERC will interact with the smart contracts? 
11. Are there any `novel` or unique `curve logic` or `mathematical models`? 
12. What `category` is the protocol ? i.e `AMM`, `Timelock`, `Bridge`, etc.
13. Is it a `fork` of a popular project ?
14. Does the project intend to go `multi-chain` ? If so, is deployment `deterministic` on different chains ?
15. Provide outline of how the scope/code will change before the audit begins, including a detailed description of any still `unimplemented parts`.
16. Describe any specific area you'd like to focus on. Eg. Try to break X invariant or Reward calculation, etc.
    
## Audit Pre-requisites
1. Make sure contracts `compile` without any errors or warnings from the compiler.
   ```sh
   # If using hardhat as a framework.
   npx hardhat compile

   # If using foundry as a framework.
   forge build
   ```
2. Run the code through a [`Spellchecker`](https://github.com/hunspell/hunspell) & [`linter`](https://github.com/protofire/solhint).
3. Have tests for "`happy path`" user stories and tests that expect reverts for actions that are supposed to fail. `All tests should be passing`.
4. Ensure there is sufficient test coverage.
   ```sh
   # If using hardhat as a framework
   npx hardhat coverage
   
   # If using foundry as a framework
   forge coverage
   ```
5. Prepare the `deploy script` and mock upgrade scripts (if applicable) and include them as part of audit scope. Deployments and upgrades are as important as runtime code and require the same amount of security attention.
6. Document all functions for more clearer developer assumptions to avoid false positives.
7. Remove any `commented/unused` code
8. Resolve any pending `TODOs`.
9.  Make sure that your project `builds correctly` on a clean system.
10. Remove any `sensitive` configurations i.e `env`, `private_keys`, `api_keys`, etc. Add exmaple `.env` (if applicable)
12. Remove any `unwanted` files not related to the project.
13. `Freeze` the code & finalize on code `commit hash`.