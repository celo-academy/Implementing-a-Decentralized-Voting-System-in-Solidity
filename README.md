## Introduction

Solidity is the main programming language for writing smart contracts in the Celo ecosystem. In this challenge, you are going to create a decentralized voting system.

## Problem Statement

Create a decentralized voting system with the following requirements:

1. The contract should allow the owner to start a new election with a list of candidates.
2. Voters should be able to cast their votes for the candidates.
3. Ensure that a voter cannot vote more than once in a single election.
4. At the end of the election, the contract should be able to tally votes and declare a winner.
5. The contract should prevent votes from being cast after the election has ended.

## Hints

- Use state variables to store the details of the election, the list of voters, and the candidates.
- The `msg.sender` global variable will come in handy to keep track of the owner of the contract.
- You may need to use mapping to prevent a voter from voting more than once.
- A `struct` can be used to encapsulate a candidate, which includes their name and vote count.
- The voting function should ensure the voter hasn't already voted, increment the candidate's vote count, and mark the voter as having voted.

## Evaluation Criteria

- **Correctness**: The contract should compile without errors and meet all the specified requirements.
- **Readability**: The contract should be easy to understand, with comments explaining the code.
- **Testability**: You should also provide examples of how to test each function of the contract.

This challenge does not cover aspects such as security, efficiency, and contract upgradability, which would be vital for a real-world voting contract.

For a comprehensive understanding of Celo smart contracts, and the Solidity language, please refer to the Celo and Solidity tutorials.

## Submission

Please reply with a link to your PR on GitHub, including your voting contract, along with any notes or comments you think are necessary to understand your design and choices. Also, provide a brief explanation about how each function of the contract should be tested.
