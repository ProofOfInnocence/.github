# Privacy Pools



## Withdrawal



Privacy Pools operate similarly to Tornado Nova. To make a withdrawal, the following steps are taken:



1. The user generates a transaction proof stating that they have a UTXO (Unspent Transaction Output).

2. The user makes an API request to the ASP (Association Set Provider) requesting the allowlist.

3. The user generates a membership proof using the Nova Folding Scheme.

4. The UI automatically downloads the membership proof.

5. The user sends the transaction proof, membership proof, and other transaction details to a Relayer.

6. The Relayer checks if the allowlists match with the subscribed ASPs.

7. The Relayer uploads the membership proof to IPFS and checks if the IPFS hash is in the transaction details.

8. If the relayer fails to upload to IPFS, user can always upload the membership proof to IPFS later.

9. The Relayer sends the transaction to the network.
