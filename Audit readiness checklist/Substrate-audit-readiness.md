## Scope Identification
1. Share the repository url of the project's public/private `repository`.
2. Share all relavent `documentation` i.e whitepapers, websites, architecture diagrams, online docs & video tutorials (if applicable).
3. How many `pallets` are there in the scope ?
4. What is the total `LOC` for all of the contracts in scope ?
5. What percentenage of `user stories` are covered in tests ?
6. What is the overall line `coverage percentage` provided by your tests?
7. Are there any `novel` or unique `curve logic` or `mathematical models`? 
8. Provide outline of how the scope/code will change before the audit begins, including a detailed description of any still `unimplemented parts`.
9. Describe any specific area you'd like to focus on. Eg. Try to break X invariant.
    
## Audit Pre-requisites
1. Make sure contracts `compile` without any errors or warnings from the compiler.
   ```sh
   cargo build --release
   ```
2. Run the code through a [`Spellchecker`](https://github.com/hunspell/hunspell) & [`rustfmt`](https://github.com/rust-lang/rustfmt).
   ```sh
   cargo fmt
   ```
3. Have tests for "`happy path`" user stories and tests that expect reverts for actions that are supposed to fail. `All tests should be passing`.
4. Resolve all issues returned by [`clippy`](https://github.com/rust-lang/rust-clippy).
   ```sh
   cargo clippy
   ```
5. Ensure all test cases pass sucessfully.
   ```sh
   cargo test
   ```
6. Ensure there is sufficient test coverage using [`tarpaulin`](https://github.com/xd009642/tarpaulin).
   ```sh
   cargo tarpaulin -v
   ```
7. Prepare the `deploy script` and mock upgrade scripts (if applicable) and include them as part of audit scope. Deployments and upgrades are as important as runtime code and require the same amount of security attention.
8. Document all functions for more clearer developer assumptions to avoid false positives.
9. Remove any `commented/unused` code
10. Resolve any pending `TODOs`.
11. Make sure that your project `builds correctly` on a clean system.
12. Remove any `sensitive` configurations i.e `env`, `private_keys`, `api_keys`, etc. Add exmaple `.env` (if applicable)
13. Remove any `unwanted` files not related to the project.
14. `Freeze` the code & finalize on code `commit hash`.