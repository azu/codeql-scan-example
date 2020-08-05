# CodeQL example

## Prepare

- Install CodeQL
- [github/vscode-codeql-starter: Starter workspace to use with the CodeQL extension for Visual Studio Code.](https://github.com/github/vscode-codeql-starter)

## Steps

```
codeql database create --language=javascript --source-root . db
codeql database analyze ./db ~/.ghq/github.com/github/vscode-codeql-starter/ql/javascript/ql/src/Security/CWE-079/Xss.ql --format=sarifv2.1.0 --output xss.sarif
```

