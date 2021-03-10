### Dependencies

- Part 1: .js/.ts related.

```shell
├── node@15.11.0
├── npm@7.6.1
├── yarn@1.22.10
└── ganache-cli@6.12.2
```

- Part 2: .py related.

```shell
├── Python@3.9.1
└── eth-brownie@1.13.3
```

1. use whatever makes you comfortable to install and manage your `nodejs` and `npm` (`nvm` recommended).
2. use whatever makes you comfortable to install and manage your `python` and `pip` (`pyenv` recommended).
3. after that, install `yarn`, `ganache-cli`, `hardhat` via `npm`; and whatever defined in `requirements.txt` via `pip`.

```shell
npm install -g yarn ganache-cli
npm install --save-dev hardhat
pip install -r requirements.txt
```

------------------------------------------------------------------------------------------------------------------------

# Tap Protocol V2 Contract Repository

## Contracts

[Tap Protocol](https://tapprotocol.com/) is a specification for tokenized asset management strategies on the ethereum
blockchain written in the Solidity programming language. We use [Hardhat](https://hardhat.org/) as a development
environment for compiling, testing, and deploying our contracts.

## Development

To use console.log during Solidity development, follow the [guides](https://hardhat.org/guides/hardhat-console.html).

## Available Functionality

### Run Hardhat EVM

`yarn chain`

### Build Contracts

`yarn compile`

To speed up compilation, install solc 0.6.10 natively with the following command.

```
brew install https://raw.githubusercontent.com/ethereum/homebrew-ethereum/06d13a8499801dc3ea4f19b2d24ed2eeb3072ebb/solidity.rb
```

### Generate TypeChain Typings

`yarn build`

### Run Contract Tests

`yarn test` to run compiled contracts

OR `yarn test:clean` if contracts have been typings need to be updated

### Run Coverage Report for Tests

`yarn coverage`

## Contributing

We highly encourage participation from the community to help shape the development of Set. If you are interested in
developing on top of Tap Protocol or have any questions, please ping us
on [Telegram](https://t.me/joinchat/Fx8D6wyprLUlM1jMVnaRdg).

## Security

### TODO: Independent Audits

### Code Coverage

All smart contracts are tested and have 100% line and branch coverage.

### Vulnerability Disclosure Policy

The disclosure of security vulnerabilities helps us ensure the security of our users.

**How to report a security vulnerability?**

If you believe you’ve found a security vulnerability in one of our contracts or platforms, send it to us by
emailing [security@tapprotocol.com](mailto:security@tapprotocol.com). Please include the following details with your
report:

* A description of the location and potential impact of the vulnerability.

* A detailed description of the steps required to reproduce the vulnerability.

**Scope**

Any vulnerability not previously disclosed by us or our independent auditors in their reports.

**Guidelines**

We require that all reporters:

* Make every effort to avoid privacy violations, degradation of user experience, disruption to production systems, and
  destruction of data during security testing.

* Use the identified communication channels to report vulnerability information to us.

* Keep information about any vulnerabilities you’ve discovered confidential between yourself and Set until we’ve had 30
  days to resolve the issue.

If you follow these guidelines when reporting an issue to us, we commit to:

* Not pursue or support any legal action related to your findings.

* Work with you to understand and resolve the issue quickly
  (including an initial confirmation of your report within 72 hours of submission).

* Grant a monetary reward based on the OWASP risk assessment methodology.

