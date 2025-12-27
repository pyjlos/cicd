## Workflows
Contains the composoite actions that application repos call
- Think of this as the "public" api that application repos call to use the pipelines

Usage of this will be something like
```
jobs:
  build:
    uses: pyjlos/cicd/.github/workflows/build-go.yaml@v1.0.5
    with:
      go-version: "1.25"
      working-directory: "./repo/"
```