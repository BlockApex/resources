## Scope Identification
1. Share the repository url of the project's public/private `repository`.
2. Share all relavent `documentation` i.e whitepapers, websites, architecture diagrams, online docs (if applicable).
4. Is there any specific libraries does the project rely on ?
5.  What is the overall line `coverage` percentage provided by your tests?
6.  Is it a `fork` of a popular project ?
7.  Provide outline of how the scope/code will change before the audit begins, including a detailed description of any still `unimplemented` parts.
8.  Describe any specific area you'd like to focus on.

## Audit Pre-requisites
1. Make sure contracts `compile` without any errors or warnings from the compiler.
   ```sh
   # If using vanilla go code
   make or go build
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
11. Remove any `unwanted` files not related to the project.
12. `Freeze` the code & finalize on code `commit hash`.