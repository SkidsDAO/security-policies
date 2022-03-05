# GitHub Actions and DevSecOps

### Github Actions: 
- Default runs Foundry tests on commit, add fuzz tests with Scribble later
- Reports gas usage upon commit
- Add Echidna to fuzz with Scribble properties
- Runs Slither and Mythril upon every commit
- Manticore will be run upon complicated logic

### DevSecOps:
#### All devs without exception must be acquainted with:
- [ConsenSys Ethereum Security Best practices](https://consensys.github.io/smart-contract-best-practices/)
- [Building Secure Smart Contracts: Development Guidelines](https://github.com/crytic/building-secure-contracts/tree/master/development-guidelines)

#### Security oriented devs/engineers must be familiar with:

It is not required to be acquainted with these techniques in the beginning but after some time ~2 to 3 weeks all devs are expected to be familiar and able with the following:

- [Program analysis with Slither, Echidna and Manticore](https://github.com/crytic/building-secure-contracts/tree/master/program-analysis)
- [Mythril](https://github.com/ConsenSys/mythril)
- [Scribble](https://docs.scribble.codes/)

Fuzz tests will be written in Scribble for incremental fuzzing with different tools i.e Foundry's fuzzer, Manticore and eventually Diligence Fuzzing.

**NB:** Devs are encouraged to get their properties reviewed by peers. Bad properties will not catch many, if any, bugs complex or otherwise.

#### Security Alerts:

- Set up Defender Sentinel with TBD Forta Agents and to monitor important functions and traffic.
- Implement OpenZeppelin Defender Admin for multi-sig functions.
#### Security Pitfalls to look out for:

- https://github.com/runtimeverification/verified-smart-contracts/wiki/List-of-Security-Vulnerabilities
