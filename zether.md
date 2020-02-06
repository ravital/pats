# Zether

Something interesting about zether

## Tools

## Efficiency

We only look at "confidential" transactions. Confidential transactions hide the amount being transferred but *not* the identities of the parties involved in the transaction. Zether also allows for "anonymous" transactions in which the indentities of the parties involved in the transaction are "hidden."

|                           |           Efficiency         |
| ------------------------- | :--------------------------: |
| Communication complexity  |                              |
| Reference string size     |                              |
| Setup time                |                              |
| Time to generate transactions |                             |
| Time to verify transactions   |                             |
| Transaction size          |                              |
| Computational resources needed |                            |
| Potential for scalability      |         Via [aggregating proofs](https://eprint.iacr.org/2017/1066.pdf) and [batch verification](https://eprint.iacr.org/2017/1066.pdf)                   |

## Security

|                           | Security                  |
| ------------------------- | :--------------------------: |
| Based on cryptography                 |       Yes&mdash;[discrete logs](https://en.wikipedia.org/wiki/Discrete_logarithm)                    |
| Based on hardware                 |            No!                  |
| Security proofs/analysis                  |                              |
| Non-standard assumptions                 |                              |
| Post-quantum               |                No!              |
| Trusted setup                |              No!                |

## Flexbility

|                           | Flexibility                 |
| ------------------------- | :--------------------------: |
| Universal reference string                 |                              |
| Support of arbitrary computation                |                              |
| Support of stateful computation                 |                              |


## Trust

|                           | Trust Level                  |
| ------------------------- | :--------------------------: |
| Trusted setup               |            No!                  |
| Any other process req. trust               |                              |
