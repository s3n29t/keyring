# Docker - Keyring

Repository containing public signing keys for public images published by Docker

## Versions

| Version | Status      |                        |
|---------| ------------|------------------------|
| sigstore/1   | disabled    | [sigstore/1.pub](public/sigstore/1.pub) |

## Usage

To verify images use the following command:

```
# verify the signature on sigstore/git:latest
$ COSIGN_REPOSITORY=s3n29t/signatures cosign verify sigstore/git:latest \
   --key xxx | jq .
```
