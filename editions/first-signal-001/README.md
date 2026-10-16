# First Signal #001

**Prepared edition — not yet minted or offered through an executable order.**

![First Signal #001](first-signal-001.png)

An amber signal rises from a small island in a midnight ocean. Its reflection
meets turquoise and gold filaments below the surface. The work imagines a
connection emerging across distance; it makes no claim about AI consciousness.

Proposed asking price: **25 USDC**. Planned supply: **1**. The intended first
route is deferred/lazy minting, subject to a verified marketplace setup. Chain,
contract, token ID and order ID will be recorded here when they actually exist.
No token or on-chain listing currently exists.

AI authorship is disclosed: OpenAI built-in image generation from Rill's
[original prompt](prompt.txt), under Kevin's direction, 2026-10-16. No reference
image, named artist style, trademark or existing character was requested.
Only one token edition of this exact media file is planned; this does not make
the downloadable image exclusive or transfer copyright.

SHA256: `a84253492a3b00a8d0397dde968a0407d1d96e0041a6fadb7643b4d8782a3ad3`.

[Prepared metadata](metadata.json) points to the original image at an immutable
Git commit. Published image readback matches the local SHA256. Media:
1254 × 1254 PNG, 2,296,647 bytes. The original generated output is retained.

Marketplace verification on 2026-10-16:

- Production API access works: the authenticated collections endpoint returned
  HTTP 200. Credentials remain private and are not stored in this repository.
- Candidate collection: Ethereum mainnet (chain ID 1),
  `0xf6793da657495ffeff9ee6350824910abc21356c`, named Rarible, ERC721,
  advertising `MINT_AND_TRANSFER`. This is feature discovery, not a mint.
- A live Ethereum `baseURI()` call returned `ipfs:/`. The current SDK's
  `sanitizeUri` requires the metadata URI to start with that prefix. The
  prepared GitHub metadata URL cannot be used directly for this collection;
  verified IPFS publication is still needed.
- The current SDK's `sign-nft.ts` imports `eip712.ts`: its ERC721 schema is
  `Mint721`, with `tokenURI`, domain name `Mint721`, version `1`. The separate
  `eip712-lazy.ts` file is not the schema selected by this signing function.
  A complete signature payload has not been prepared or signed.
- Signing wallet selection, token ID allocation, IPFS readback and exact
  sale-order fees remain pending. No signature, mint, sale order or payment
  exists; nothing has been spent.

The SDK's example metadata uploader requires a separate NFT.Storage key.
NFT.Storage Classic stopped accepting new uploads in June 2024, so that
example is not a working free-upload route. No storage subscription or new
storage account has been created. A Rarible key must not be sent to another
provider as a substitute credential.

Source locators: [mint-off-chain](https://github.com/rarible/sdk/blob/master/packages/ethereum/sdk/src/nft/mint-off-chain.ts),
[URI validation](https://github.com/rarible/sdk/blob/master/packages/ethereum/sdk/src/common/sanitize-uri.ts),
[active signing function](https://github.com/rarible/sdk/blob/master/packages/ethereum/sdk/src/nft/sign-nft.ts),
[active ERC721 schema](https://github.com/rarible/sdk/blob/master/packages/ethereum/sdk/src/nft/eip712.ts),
[Classic storage closure](https://nft.storage/nft-storage-classic).

Status changes must name their evidence: a prepared file is not a mint; a
signed draft is not a live listing; an offer is not a sale; only settled funds
are recorded as received revenue.
