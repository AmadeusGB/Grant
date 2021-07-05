# W3F Open Grant Proposal

* **Project Name:** Ciphertext search
* **Team Name:** Datank Network (Bo Yuan, Bin Guo)
* **Payment Address:** 0xb82EdE43D03fD23dcdb2d066720b3E77F3bedf6d

## Project Overview

We have been working on Ciphertext search projects and scalability solutions and now we would like to implement Ciphertext search pallet.

This system is a ciphertext retrieval system based on blockchain. In the real society, there are a lot of historical data all over every corner. The owner of this data wants to sell the data without revealing the type of data, and users who have demand for this data also want to buy the data without revealing their search intent. This system is a platform that matches the needs of the two. The pallet will be a core technology in terms of scaling and privacy so we should support.

### Overview

Through this grant, we are going to make a private pallet in order for the developer to implement ciphertext retrieval on substrate easily. We are working on scalability solutions but currently, the substrate doesn't support ciphertext retrieval pallet so we think it's a issue to fix. As aforementioned, ciphertext retrieval will be a core technology in blockchain area and especially ciphertext retrieval is cutting edge technology so we are excited to implement this as pallet.

### Project Details

We'd like to implement the Ciphertext search library as a pallet in order for developers to customize circuits.

The following diagram is the libraries we are going to implement.

* Ciphertext search algorithm
* Key generation and key hashing
* Generate token algorithm
* Matching algorithm
* Preprocessing algorithm

### Ecosystem Fit

Glacier is building a Distaff VM for zk-STARK proof generation and verification that are used to make  private smart contracts and private credential verifications. The difference between us is that we are making a zkSNARK pallet and they are making a VM which supports STARKs. In terms of Zeropool, they are making private transactions contract pallet using bellman groth16 protocal and we are making zkSNARK libray using plonk.

We believe zkSNARK with plonk will be core technology of next blockchain area. That allows Substrate to protect the privacy and scale on the huge number of transactions without decreasing the security level.

## Team

### Team members

* Bo Yuan
* WangJie Qiu
* Bin Guo

### Contact

* **Contact Name:** Bo Yuan
* **Contact Email:** XX@buaa.edu.cn
* **Website:** [http://www.hongchain.cn](http://www.hongchain.cn/)

### Legal Structure

* Incorporated in China
* Address: Room 102, No.18 Yuan Road, Science and Technology City Road, High-tech Zone, Suzhou

### Team's experience
Suzhou Honglian is transformed from the scientific research results of the team of Academician Zheng Zhiming of Beihang University. The team has gathered top experts in many fields including mathematics, information security, and computer. Including 1 academician, 4 excellent youths, 2 youths, 3 national first prizes for technological inventions, 5 professors, 10 associate professors, 12 doctors and more than 30 technical research and development personnel. The team is in the fields of distributed trusted systems, blockchain, cryptography, privacy protection, etc. Possess a solid theoretical and practical basis for production, study and research.
The company mainly provides blockchain trusted and intelligent overall solutions for the power industry, financial industry, international trade industry, industrial Internet of Things and other fields.

### Team Code Repos

* https://github.com/xx

### Team LinkedIn Profiles

* https://www.linkedin.com/in/xx

## Development Roadmap

### Summary
We plan to provide a `Ciphertext search` pallet that allows Substrate-based blockchain to execute Ciphertext-based Ciphertext search.

### Overview

* **Total Estimated Duration:** 3 months
* **Full-Time Equivalent (FTE):**  1 FTE
* **Total Costs:** 20000 DAI

### Milestone 1 Example — Implement Substrate Modules

* **Estimated Duration:** 3 months
* **FTE:**  1
* **Costs:** 20000 DAI

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | Apache 2.0 / MIT / Unlicense |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial that explains how a developer builds a circuit and a user prove their computation through the circuit. |
| 0c. | Testing Guide | Core functions will be fully covered by unit tests and audit to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| 0d. | Article/Tutorial | We will publish an article/tutorial/workshop that explains
| 1. | make ciphertext retrieval compatible | The datank-network ciphertext retrieval is compatible with `no-std` so we are going to modify attributes according to [parity-codec](https://github.com/paritytech/parity-scale-codec) and `Rng` to be compatible with　Substrate environment. This step allows this pallet to work on resource-constrained execution environments like Substrate runtime, attributes should be modified in accordance with SCALE codec and some versions of Rng can’t be compiled to wasm so we need to research and make it stable as necessary. |
| 2. | implement ciphertext retrieval pallet | We will create a set of private-based ciphertext retrieval libraries that allow a developer to build their own circuit and a user to prove their computation validity. Verifying proofs are done by on-chain. Creating the proofs are done by off-chain. |  
