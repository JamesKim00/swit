# On Implementing Blockchain Technology

## Contents

1. Benefits of the technology
1. The downsides
1. Conclusion

- Sources

## 1. The Benefits of the Technology

### General Benefits

> #### Provides a trustless environment
>
> In a decentralized blockchain network, no one has to know or trust anyone else.
> Each member in the network has a copy of the exact same data in the form of a distributed ledger.
> If a member’s ledger is altered or corrupted in any way, it will be rejected by the majority of the members in the network.

> #### Improves data reconciliation
>
> Companies often exchange data with their partners.
> This data, in turn, is typically transformed and stored in each party’s data silos, only to resurface
> when it needs to be passed downstream. Each time the data is transformed, it opens up opportunities for data
> loss or incorrect data to enter the workstream. By having a decentralized data store, every entity has access
> to a real-time, shared view of the data.

> #### Reduces points of weakness
>
> Decentralization can reduce points of weakness in systems where there may be too much reliance on specific actors.
> These weak points could lead to systemic failures, including failure to provide promised services or
> inefficient service due to the exhaustion of resources, periodic outages, bottlenecks, lack of sufficient
> incentives for good service, or corruption.

> #### Optimizes resource distribution
>
> Decentralization can also help optimize the distribution of resources so that promised services are provided
> with better performance and consistency, as well as a reduced likelihood of catastrophic failure.

**(Source: [here](https://aws.amazon.com/blockchain/decentralization-in-blockchain/))**

### Benefits for the Healthcare Industry

> #### Better Patient Data Management and Sharing
>
> Enables the owner of medical data to maintain its privacy while also providing a vehicle for patients, doctors, and
> healthcare providers to share the same information rapidly and securely
> In addition, can reduce patient documentation errors and issues resulting from conflicting data among medical practitioners.
> Moreover, blockchain technology, in combination with smart contracts, can set parameters that only allow access to
> patient data in compliance with a patient’s consent policy.

> #### More Payment Efficiency
>
> There are no third-party payment vendor services with blockchain as it relates to fees, meaning once a service is provided,
> the healthcare provider can receive a direct transfer of the agreed-upon cryptocurrency directly to their wallet,
> which provides a secure, transparent, fast, and traceable method of payment.

> #### Data Security and Electronic Health Records
>
> Current recordkeeping systems can be vulnerable to cyberattacks as data breaches result in significant financial losses to
> healthcare practitioners and organizations, reduce trust, and damage brand integrity.
> Blockchain, however, can be used to create standard security protocols, provide end-to-end encryption, prevent unauthorized
> access to data while in transit, and verify the integrity of software downloads.
> In addition, decentralizing sensitive data makes it harder, if not impossible, for hackers to penetrate data storage systems.

> #### Distributed storage
>
> Rather than storing data in a single location, blockchain is stored across a network.
> That means if a healthcare organization suffers a massive data breach, the entire chain isn't compromised.

> #### Password-protection
>
> Blockchain technology requires a private key to grant access. Patients could allow access to trusted parties
> like physicians, but it would make unauthorized access nearly impossible.

> #### Trust
>
> The mathematical equations that compose blockchain help preserve the integrity and quality of data across the network.

**(Sources:
[Link 1](https://www.jdsupra.com/legalnews/3-ways-that-blockchain-can-help-the-1711780/),
[Link 2](https://www.fiercehealthcare.com/privacy-security/3-reasons-blockchain-answer-to-ehr-interoperability-and-security)
)**

## The Downsides

### Difficulty of Implementation and Development [(Source)](https://jimmysong.medium.com/why-blockchain-is-hard-60416ea4c5c)

> #### Development is stricter and slower
>
> > Creating a provably consistent system is not an easy task. A small bug could corrupt the entire database or cause some
> > databases to be different than other ones. Of course, a corrupted or split database no longer has any consistency guarantees.
> > Furthermore, all such systems have to be designed from the outset to be consistent. There is no “move fast and break things”
> > in a blockchain. If you break things, you lose consistency and the blockchain becomes corrupted and worthless.

> > Fixing or starting over and moving on a database would be easy enough to do in a centralized system,
> > but this is very difficult in a decentralized one. You need consensus, or the agreement of all players in the system,
> > in order to change the database. The blockchain has to be a public resource that’s not under the control of a single entity
> > (decentralized), or the entire effort is a very expensive way to create a slow, centralized database.

> #### Maintenance is very costly
>
> > A traditional centralized database only needs to be written to once. A blockchain needs to be written to thousands of times.
> > A traditional centralized database needs to only checks the data once. A blockchain needs to check the data thousands of times.
> > A traditional centralized database needs to transmit the data for storage only once. A blockchain needs to transmit the data thousands of times.

> > The costs of maintaining a blockchain are orders of magnitude higher and the cost needs to be justified by utility.
> > Most applications looking for some of the properties like consistency and reliability can get such things
> > for a whole lot cheaper utilizing integrity checks, receipts and backups.

> #### Scaling is really hard
>
> Scaling is at least several orders of magnitude harder than in a traditional centralized system.
> The reason is obvious. The same data has to live in hundreds or thousands of places than in a single place.
> The overhead of transmission, verification and storage is enormous as every single copy of the database must
> pay them instead of those costs being paid just once in a traditional, centralized database.
> You can, of course, reduce the
> burden by reducing the number of nodes. But then at that point, why do you need a decentralized system at all?
> Why not just make a centralized database if scaling costs are the main concern?

### Data Storage

> #### Large Amounts of Data [(Source)](https://www.jdsupra.com/legalnews/3-ways-that-blockchain-can-help-the-1711780/)
>
> Private healthcare data tends to be highly voluminous, which could impact the functionality of the blockchain.
> Blockchains suffering from network slowdown due to large storage could prevent an obstacle to mass adoption in the
> healthcare industry.

> #### The Inherent Nature of Blockchains [(Source)](https://www.fiercehealthcare.com/tech/private-blockchain-explained-what-it-what-it-isn-t-and-how-to-manage-your-hipaa-expectations)
>
> > Blockchains are not databases. Their role is to disseminate data, not store it. The structure of a blockchain actually makes it
> > very expensive to keep information on-chain—a reason use cases so far have mostly used blockchains for provenance data,
> > which are quite small.

> > EHRs, meanwhile, aren't exactly light on data. It's conceivable the health information of even a single individual would be
> > too much to store on-chain, especially if it includes multiple large files like high-resolution images. There's no way any
> > blockchain developed so far would be able to contain the data housed in a titanic EHR system.

> > "It's just too expensive, I mean that's a showstopper right there," Smolenski said."You know, if you take a photo from a
> > standard camera today, that's 8 MB. If you were going to store 1 MB on a shared network it would cost you about $7,000,
> > so it's not even practical."

### Compliance with HIPAA

> #### Storing Patient Data on a Decentralized Network [(Source)](https://www.jdsupra.com/legalnews/3-ways-that-blockchain-can-help-the-1711780/)
> HIPAA compliance may be an issue when storing private patient data on a decentralized network designed to be transparent.
> Storage of private patient data on a public ledger presents a risk of sensitive data being exposed.
> There is an argument that use of blockchain technology alone is not enough to ensure the requisite level of privacy.

> #### The Encryption Method of Blockchain [(Source)](https://www.anonos.com/blockchain-and-big-data-privacy-in-healthcare) [(Source 2)](https://masur.com/lawtalk/is-blockchain-hipaa-compliant/)
>
> Blockchain is premised on mathematically derived pseudonyms for distributed ledger verification and the
> HIPAA Privacy Rule prohibits use of mathematically-derived pseudonyms because of potential re-identification of
> de-identified protected health information (PHI).
> This limitation on the use of mathematically-derived pseudonyms as re-identification codes for de-identified information
> effectively makes blockchain non-HIPAA compliant [(Page 53233)](https://www.gpo.gov/fdsys/pkg/FR-2002-08-14/pdf/FR-2002-08-14.pdf).

## Conclusion

There are, of course, many ways to counteract the downsides such as using blockchain together with alternate database. However, I firmly believe the downsides, even with the possible solutions, still outweigh the potential benefits the technology may bring.

## Sources

- https://jimmysong.medium.com/why-blockchain-is-hard-60416ea4c5c
- https://aws.amazon.com/blockchain/decentralization-in-blockchain/
- https://www.jdsupra.com/legalnews/3-ways-that-blockchain-can-help-the-1711780/
- https://www.hipaajournal.com/blockchain-medical-records/
- https://www.anonos.com/blockchain-and-big-data-privacy-in-healthcare
- https://masur.com/lawtalk/is-blockchain-hipaa-compliant/
- https://www.fiercehealthcare.com/privacy-security/3-reasons-blockchain-answer-to-ehr-interoperability-and-security
- https://www.fiercehealthcare.com/tech/private-blockchain-explained-what-it-what-it-isn-t-and-how-to-manage-your-hipaa-expectations
- https://www.hipaavault.com/resources/blockchain-technology-and-the-future-of-healthcare/?amp
