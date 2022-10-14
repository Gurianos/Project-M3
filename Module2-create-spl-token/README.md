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
yarn upgrade
yarn add @solana/web3.js
yarn add @metaplex-foundation/mpl-token-metadata
yarn add @metaplex-foundation/js
yarn add @solana/spl-token
yarn add fs



Open tsconfig.json and uncomment (or add) this to your file: 
"resolveJsonModule": true
Also double check that esModuleInterop is set to true to allow for us to use imports. 
and add at the end 



ts-node wallet.ts

Here publicKey is a wallet publicKey. It will returns all metadata owned by a wallet.


guideSecret.json create when launch 