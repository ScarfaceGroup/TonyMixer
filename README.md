Tony’s Dry-Cleaning Service - The DApp Mixer 

Tony’s Dry-Cleaning Service is a non-custodial privacy solution based on zkSNARKs built on the Binance Smart Chain. It enhances transaction privacy by breaking the on-chain link between source and destination addresses. It uses a smart contract that accepts BNB and $TONY deposits that can be withdrawn by a different address. Whenever tokens are withdrawn by the new address, there is no way to link the withdrawal to the deposit, ensuring complete privacy.

To make a deposit, the user generates a secret and sends its hash (called a commitment) along with the deposit amount to the Tony’s Dry-Cleaning Service smart contract. The contract accepts the deposit and adds the commitment to its list of deposits.

Later, when the user decides to make a withdrawal, they should provide a proof that they possess a secret to an unspent commitment from the smart contract’s list of deposits. zkSnark technology allows this to happen without revealing which exact deposit corresponds to this secret. The smart contract checks the proof and transfers deposited funds to the address specified for withdrawal. An external observer will be unable to determine from which deposit this withdrawal originated.

Each time our cleaning service is used, 1% of the $TONY tokens spent as fees are permanently burned.

You can read more about it in this Medium article (coming soon)

Specs
Deposit gas cost: 1088354 (43381 + 50859 * tree_depth)
Withdraw gas cost: 301233
Circuit Constraints = 28271 (1869 + 1325 * tree_depth)
Circuit Proof time = 10213ms (1071 + 347 * tree_depth)
