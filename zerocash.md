# [Zerocash](http://zerocash-project.org/media/pdf/zerocash-extended-20140518.pdf)
[Zcash](https://z.cash) uses the [Zerocash protocol](http://zerocash-project.org/media/pdf/zerocash-extended-20140518.pdf). However, it's important to note that there are some changes Zcash has made to the Zerocash protocol (which can be found in the [protocol specification](https://github.com/zcash/zips/blob/master/protocol/protocol.pdf)). 
## Tools

## Efficiency

The authors provide timings for a few different machine setups. For readers interested in further performance details, we suggest looking at the [paper](http://zerocash-project.org/media/pdf/zerocash-extended-20140518.pdf). Zerocash specifies two transaction types&mdash;"Mint" and "Pour." Our chart below only includes details for "Pour" transactions which make use of zk-SNARKs.

|                           |           Efficiency         |
| ------------------------- | :--------------------------: |
| [Communication complexity](https://en.wikipedia.org/wiki/Communication_complexity)  |                              |
| Reference string size     |              ; 896 MiB              |
| Setup time                |       ; 5 mins 17 secs                   |
| Time to generate transactions |             ; 2 mins 2.01 secs                |
| Time to verify transactions   |             ; 5.7 ms                |
| Transaction size          |         Constant; 996 B               |
| Computational resources needed |  Intel i7-4770 at 3.40GHz with 16GB RAM and 1 thread     |
| Potential for scalability      |                         |

## Security

|                           | Security                  |
| ------------------------- | :--------------------------: |
| Based on cryptography                 |         Yes&mdash;discrete logs                 |
| Based on hardware                 |         No!                    |
| ZKP                       |   [zk-SNARKs](https://eprint.iacr.org/2013/879)     |
| Security proofs/analysis                  |         Yes!                   |
| Non-standard assumptions                 |      [Knowledge-of-Exponent](https://medium.com/@VitalikButerin/zk-snarks-under-the-hood-b33151a013f6)                        |
| [Post-quantum](https://en.wikipedia.org/wiki/Post-quantum_cryptography)               |       No                   |
| [Trusted setup](https://zcoin.io/ufaqs/what-is-trusted-setup/)                |            Yes         |

## Flexbility

|                           | Flexibility                 |
| ------------------------- | :--------------------------: |
| [Universal reference string](https://docs.zkproof.org/assets/docs/reference-v0.2.pdf)      |              No               |
| Support of arbitrary computation                |        No                    |
| Support of stateful computation                 |    No                    |
| Suggested applications                 |                             |


## Trust

|                           | Trust Level                  |
| ------------------------- | :--------------------------: |
| [Trusted setup](https://zcoin.io/ufaqs/what-is-trusted-setup/)               |         Yes               |
| Any other process req. trust               |                              |

