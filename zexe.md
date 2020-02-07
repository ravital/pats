# Zexe


## Tools

## Efficiency
|                           |           Efficiency         |
| ------------------------- | :--------------------------: |
| [Communication complexity](https://en.wikipedia.org/wiki/Communication_complexity)  |                              |
| Reference string size     |                            |
| Setup time                |                              |
| Time to generate transactions |                             |
| Time to verify transactions   |   Constant;                          |
| Transaction size          |      Linear (in number of input and output records); [968 bytes for 2 input/output records](https://eprint.iacr.org/2018/962.pdf)                      |
| Computational resources needed |  Specialized for generation of computation ([Intel Xeon 6138 CPU at 3.0 Ghz, 252GB of RAM](https://eprint.iacr.org/2018/962.pdf))                          |
| Potential for scalability      |                         |

## Security

|                           | Security                  |
| ------------------------- | :--------------------------: |
| Based on cryptography                 |                          |
| Based on hardware                 |            No!                 |
| ZKP                       |         SNARK     |
| Security proofs/analysis                  |      Yes&mdash;rigorous!                     |
| Non-standard assumptions                 |                              |
| [Post-quantum](https://en.wikipedia.org/wiki/Post-quantum_cryptography)               |       No                    |
| [Trusted setup](https://zcoin.io/ufaqs/what-is-trusted-setup/)                |        Yes                  |

## Flexbility

|                           | Flexibility                 |
| ------------------------- | :--------------------------: |
| [Universal reference string](https://docs.zkproof.org/assets/docs/reference-v0.2.pdf)                 |                              |
| Support of arbitrary computation                |                            |
| Support of stateful computation                 |                        |
| Suggested applications                 |      Decentralized Exchanges                       |


## Trust

|                           | Trust Level                  |
| ------------------------- | :--------------------------: |
| [Trusted setup](https://zcoin.io/ufaqs/what-is-trusted-setup/)               |     Yes                   |
| Any other process req. trust               |      "[Delegable DPC](https://eprint.iacr.org/2018/962.pdf)"&mdash;allows user to delegate the computation to a worker                       |

