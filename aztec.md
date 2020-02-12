# [Aztec](https://github.com/AztecProtocol/AZTEC/blob/master/AZTEC.pdf)

## Tools

## Efficiency

|                           |           Efficiency         |
| ------------------------- | :--------------------------: |
| [Communication complexity](https://en.wikipedia.org/wiki/Communication_complexity)  |                              |
| Reference string size     |       Linear ([in cardinality of range used by range proof](https://github.com/AztecProtocol/AZTEC/blob/master/AZTEC.pdf))                     |
| Setup time                |                              |
| Time to generate transactions |                             |
| Time to verify transactions   |       Constant                      |
| Transaction size          |                            |
| Computational resources needed |                            |
| Potential for scalability      |                         |

## Security

|                           | Security                  |
| ------------------------- | :--------------------------: |
| Based on cryptography                 |       Yes&mdash;[discrete logs](https://en.wikipedia.org/wiki/Discrete_logarithm)                   |
| Based on hardware                 |                             |
| ZKP                       |    [Sigma Protocol](https://en.wikipedia.org/wiki/Proof_of_knowledge#Sigma_protocols)    |
| Security proofs/analysis                  |        Some important analysis missing*                    |
| Non-standard assumptions                 |       Potentially [random oracle](https://en.wikipedia.org/wiki/Random_oracle)                       |
| [Post-quantum](https://en.wikipedia.org/wiki/Post-quantum_cryptography)               |      No                     |
| [Trusted setup](https://zcoin.io/ufaqs/what-is-trusted-setup/)                |         Yes                 |

## Flexbility

|                           | Flexibility                 |
| ------------------------- | :--------------------------: |
| [Universal reference string](https://docs.zkproof.org/assets/docs/reference-v0.2.pdf)                 |                              |
| Support of arbitrary computation                |           No                 |
| Support of stateful computation                 |        No                |
| Suggested applications                 |            Just asset transfers*                 |


## Trust

|                           | Trust Level                  |
| ------------------------- | :--------------------------: |
| [Trusted setup](https://zcoin.io/ufaqs/what-is-trusted-setup/)               |       Yes                 |
| Any other process req. trust               |                              |

