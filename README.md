# PATS Framework

## Framework

|                           | Efficiency[[0]](#Efficiency) | Security[[1]](#Security) | Flexibility[[2]](#Flexibility) | Trust Level Needed[[3]](#Trust-Level) |
| ------------------------- | :--------------------------: | :----------------------: | :----------------------------: | :-----------------------------------: |
| [Zether](./zether.md)     |           Mediocre           |           High           |             Medium             |                  Low                  |
| [Aztec](./aztec.md)       |          Efficient           |          Low-Medium          |              Low               |                 High                  |
| [Zexe](./zexe.md)         |       Fairly Efficient       |          Medium          |          Medium-High           |                 High                  |
| [Zerocash](./zerocash.md) |       Fairly Efficient       |          Medium          |              Low               |                 High                  |

## Purpose

Private asset transfer solutions (PATS) are arguably the most popular application of ZKPs currently. However, with so many solutions on offer, it is easy for a non-expert in the space to feel overwhelmed and struggle to understand the differences between them. While there has been effort in the ZKProof community towards creating a conceptual framework for comparing and contrasting different ZKP protocols, there has yet to have been a clear conceptual framework suggested for comparing private asset transfer solutions.

We will explain how we can use some of the properties of ZKPs (from ZKProof Community Reference Version 0.2)—namely security, efficiency, and trust—to effectively compare private asset transfer solutions. We also introduce the concept of [flexibility](#Flexibility) in discussing private asset transfer solutions which incorporates the notions of preprocessing, CRS, and SRS. In light of these 4 properties, we compare some recent solutions. With new notions and features being added to ZKPs and private asset transfer solutions—such as the notion of updateable trust (e.g. Sonic) and allowing for private computation beyond transactions (e.g. Zether, Zexe)—we hope that the introduction of the notion of flexibility will capture new developments in the space.

As PATS are introduced, we will add to this table. We also hope that the creation of this framework will lead to a larger conversation within the ZKProof community about how best to discuss PATS with a broader audience.

## Definitions

Where possible, we incorporate the definitions of the ZKProof Community Reference document. There has been increasing interest in allowing for computation beyond pure transactions in PATS (e.g. "smart contracts" in Ethereum). Thus, we introduce the concept of "flexbility" which measures if the scheme supports more complex logic.

### Efficiency

Efficiency includes the following properties:

- setup cost (time, size)
- total communication cost (time, size)
- time to generate transaction
- time to verify transactiion
- computational resources required to achieve stated times
- potential for scalability (e.g. through batching, parallelization)

### Security

Security includes the following:

- hardness assumption used (preferably the hardness assumption used is well-understood and weak; security should be based solely on cryptography)
- security proofs
- use of trusted setup (trusted setups weaken security)
- post-quantum (ideal if scheme is post-quantum)

### Flexibility

Flexibility includes the following:

- a "universal" common reference string (this means the reference string is independent of the relation so we wouldn't need to generate a new reference string to prove a new statement each time)
- support of arbitrary computation (can we express more complex logic with our scheme? e.g. voting)
- support of "stateful" computation (can incorporate some notion of state/time)

### Trust Level

Trust level indcates if we must trust any party to be "honest" to ensure the system is secure (i.e. trusted setup process).

Schemes that use structured reference strings, for example, require a higher degree of trust than those that don't. If the party involved in the trusted setup process behaves maliciously, he/she can violate the "zero-knowledge" aspect of the system. Some recent ZKP schemes use "updateable" structured reference strings which require less trust than schemes with a static trusted setup, but more trust than ZKP scheme with no trusted setup whatsoever.

# Contributions

We welcome all contributions. Please open an issue first so we can discuss your changes.
