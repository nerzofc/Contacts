# Nerzo Platform Contracts

Nerzo is a web3 application leveraging [Thirdweb](https://thirdweb.com/) integration to facilitate seamless blockchain-based interactions through smart contracts. Our platform is meticulously designed with a focus on performance and user experience. As proud participants in the Thirdweb Startup Program, we build on the robust infrastructure provided by [Thirdweb](https://thirdweb.com/), utilizing their suite of advanced pre-built smart contracts.

## Smart Contracts

Our project utilizes the following smart contracts from [Thirdweb](https://thirdweb.com/):

- **OpenEditionERC721**: [Version 5.0.1](https://thirdweb.com/thirdweb.eth/OpenEditionERC721/5.0.1) - This contract allows for the creation and management of open edition NFTs, enabling users to mint and trade digital assets securely.

- **StakeERC20**: [Version 5.0.1](https://thirdweb.com/thirdweb.eth/TokenStake) - This contract allows users to stake their ERC-20 tokens and receive ERC-20 tokens as staking rewards (different from the staked tokens).

- **StakeERC721**: [Version 5.0.1](https://thirdweb.com/thirdweb.eth/NFTStake) - This contract allows users to stake their ERC-721 NFTs and receive ERC-20 tokens as staking rewards.

- **Token**: [Version 5.0.1](https://thirdweb.com/thirdweb.eth/TokenERC20) - The Token contract is suited for creating a digital currency and is compliant with the ERC20 standard.

- **Managed Account Factory**: [Version 1.57.27](https://thirdweb.com/thirdweb.eth/ManagedAccountFactory) - This contract allows deploying upgradeable smart wallets for users, with the ability to push updates to all users.

All the contracts are available in the [Thirdweb GitHub repository](https://github.com/thirdweb-dev/contracts).


## Usage

To use the Nerzo platform, you need to interact with the smart contracts deployed on the blockchain. The following example demonstrates how to call a smart contract using the `Web3Button` component.

## Example: How We Call the Smart Contract

```jsx
<Web3Button
  contractAddress="0x3898c51D4DCd03D8aF57A714DD1Bf667e1AfFCAD"
  action={async (contract) => {
    await contract.erc721.claim(value);
  }}
  onSuccess={(result) => alert("Success!")}
>
  Mint
</Web3Button> 
```

## License

[Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0.txt)
