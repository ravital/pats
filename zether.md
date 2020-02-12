# [Zether](https://eprint.iacr.org/2019/191.pdf)

Something interesting about zether

## Tools

## Efficiency

We only look at "confidential" transactions. Confidential transactions hide the amount being transferred but *not* the identities of the parties involved in the transaction. Zether also allows for "anonymous" transactions (via the use of [ring signatures](https://en.wikipedia.org/wiki/Ring_signature)) in which the indentities of the parties involved in the transaction are "hidden."

|                           |           Efficiency         |
| ------------------------- | :--------------------------: |
| [Communication complexity](https://en.wikipedia.org/wiki/Communication_complexity)  |      Logarithmic;                        |
| Reference string size     |               Linear (needed by Verifier);               |
| Setup time                |                              |
| Time to generate transactions |            Linear (in bit length of range);                 |
| Time to verify transactions   |       Linear (in bit length of range);                      |
| Transaction size          |            Logarithmic (in the [witness](https://en.wikipedia.org/wiki/NP_(complexity)) size); concretely, [1472 bytes](https://eprint.iacr.org/2019/191.pdf) when optimized to work with Ethereum                  |
| Computational resources needed |   Minimal (from [Bulletproofs](https://eprint.iacr.org/2017/1066.pdf): Intel i7-6820HQ, single thread, <100MB memory)                         |
| Potential for scalability      |         Via [aggregating proofs](https://eprint.iacr.org/2017/1066.pdf) and [batch verification](https://eprint.iacr.org/2017/1066.pdf)                   |

## Security

|                           | Security                  |
| ------------------------- | :--------------------------: |
| Based on cryptography                 |       Yes&mdash;[discrete logs](https://en.wikipedia.org/wiki/Discrete_logarithm)                    |
| Based on hardware                 |            No!                  |
| ZKP                       |        Bulletproofs and [Sigma protcols](https://en.wikipedia.org/wiki/Proof_of_knowledge#Sigma_protocols) ([Sigma-Bullets](https://eprint.iacr.org/2019/191.pdf)) |
| Security proofs/analysis                  |         Yes&mdash;rigorous!                     |
| Non-standard assumptions                 |        Potentially [random oracle](https://en.wikipedia.org/wiki/Random_oracle)                      |
| [Post-quantum](https://en.wikipedia.org/wiki/Post-quantum_cryptography)               |                No            |
| [Trusted setup](https://zcoin.io/ufaqs/what-is-trusted-setup/)                |              No!                |

## Flexbility

|                           | Flexibility                 |
| ------------------------- | :--------------------------: |
| [Universal reference string](https://docs.zkproof.org/assets/docs/reference-v0.2.pdf)    |       Yes!                       |
| Support of arbitrary computation                |         No&mdash;additive relations only                   |
| Support of stateful computation                 |     Yes!                      |
| Suggested applications                 |    [Sealed-bid auctions, stake voting](https://eprint.iacr.org/2019/191.pdf)                          |


## Trust

|                           | Trust Level                  |
| ------------------------- | :--------------------------: |
| [Trusted setup](https://zcoin.io/ufaqs/what-is-trusted-setup/)               |            No!                  |
| Any other process req. trust               |          No!                    |
