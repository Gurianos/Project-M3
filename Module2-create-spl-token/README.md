Some guide usable :

// https://www.npmjs.com/package/@metaplex-foundation/mpl-token-metadata
// https://metaplex-foundation.github.io/metaplex-program-library/docs/token-metadata/index.html
// https://metaplex-foundation.github.io/metaplex-program-library/docs/token-metadata/index.html#CreateMetadataAccountV3InstructionArgs
// https://www.youtube.com/watch?v=DQbt0-riooo
// https://www.quicknode.com/guides/solana-development/how-to-create-a-fungible-spl-token-with-the-new-metaplex-token-standard

npm install @metaplex-foundation/mpl-token-metadata --save
or
yarn init

tsc --init


yarn install

yarn add @solana/web3.js
yarn add @metaplex-foundation/mpl-token-metadata
yarn add @metaplex-foundation/js
yarn add @solana/spl-token
yarn add fs

// if needed
yarn upgrade

// Open tsconfig.json and uncomment (or add) this to your file: 
"resolveJsonModule": true
// Also double check that esModuleInterop is set to true to allow for us to use imports. 

//launch the wallet creation
ts-node wallet.ts
// guideSecret.json is created and available in your repository project

// your wallet is ready to use, 
use solana config set keypair=<guideSecret.json path>
// your wallet is now ready to use, 

Here publicKey is a wallet publicKey. It will returns all metadata owned by a wallet

now configure mint.ts with your RPC, metadata, token infos 
configure your RPC endpoint, the number of token,  decimals, path of your token image.
beug ? : if you choose 0 as decimal you will have your SPL token available on the NFT phantomWallet after transfer.

// launch the mint.ts will create the token address , the token account, transfert the metadata & link the image.
ts-node mint.ts // to mint your tokens

spl-token accounts -v // will gave you the token address and and the token accounts.
transfert it to your phantom wallet address


spl-token transfer --fund-recipient <token address> 1000 <phantom wallet address>


we can now go to the Candy machine install and configurations using Sugar :)