# Cowsay Action

> The cowsay GitHub Action written in JavaScript

[![Build Status](https://github.com/octokit/cowsay-action/workflows/Test/badge.svg)](https://github.com/octokit/cowsay-action/actions)

## Usage

```yml
name: Hello world!
on:
  push:
    branches:
      - master

jobs:
  sayHelloWorld:
    runs-on: ubuntu-latest
    steps:
      - uses: gr2m/cowsay-action@v1.x
        with:
          text: "Hello"
```

Will log

```
 _______
< Hello >
 -------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```

## License

[ISC](LICENSE)

## Privacy

This Action contacts Chainguard's licensing server to verify authorization. Connection metadata (IP address, GitHub repository identifier, timestamp, and any metadata encoded in the auth token) is transmitted to Chainguard, Inc. even if authorization is denied in accordance with our [Privacy Notice](https://www.chainguard.dev/legal/privacy-notice)
