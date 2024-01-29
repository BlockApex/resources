## Scope Identification
1. Share the repository url of the project's public/private `repository`.
2. Share all relavent `documentation` i.e whitepapers, websites, architecture diagrams, online docs (if applicable).
3. What framework was used to build the chain ? i.e [`ignite`](https://docs.ignite.com/), [`cosmos-sdk`](https://v1.cosmos.network/sdk)
4. How many `modules` are there in the scope ?
5. Is there any specific libraries does the project rely on ?
6.  What is the overall line `coverage` percentage provided by your tests?
7.  Does the project implements `IBC` as native module ?
8.  Does the project support `wasm` module ?
9.  Is it a `fork` of a popular project ?
10. Provide outline of how the scope/code will change before the audit begins, including a detailed description of any still `unimplemented` parts.
11. Describe any specific area you'd like to focus on.

## Audit Pre-requisites
1. Make sure contracts `compile` without any errors or warnings from the compiler.
   ```sh
   # If using vanilla go code
   make or go build
   
   # If using ignite-cli
   ignite chain build
   ```
2. Apply code formatting `gofmt`.
   ```sh
   gofmt -s -w
   ```
3. Resolve all linting issues [`golang-ci`](https://github.com/golangci/golangci-lint).
   ```sh
   golangci-lint run
   ```
4. Resolve issues by go [`vet`](https://pkg.go.dev/cmd/vet).
   ```sh
   go vet
   ```
5. Ensure there is sufficient test coverage.
   ```sh
   go test -cover
   ```
6. Document all functions for more clearer developer assumptions to avoid false positives.
7.  Remove any `commented/unused` code
8.  Resolve any pending `TODOs`.
9.  Make sure that your project `builds correctly` on a clean system.
10. Remove any `sensitive` configurations (if applicable).
11. Remove any `unwanted` file not related to the project.
12. `Freeze` the code & finalize on code `commit hash`.