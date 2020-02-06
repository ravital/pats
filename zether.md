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
| Potential for scalability      |                            |

## Security

|                           | Security                  |
| ------------------------- | :--------------------------: |
| Based on cryptography                 |       Yes&mdash;[discrete logs](https://en.wikipedia.org/wiki/Discrete_logarithm), specifically [Decisional Diffie-Hellman](https://en.wikipedia.org/wiki/Decisional_Diffie%E2%80%93Hellman_assumption)                    |
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
| Trusted setup               |                              |
| Any other process req. trust               |                              |
