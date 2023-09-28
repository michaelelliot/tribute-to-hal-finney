# A Tribute to Hal Finney

This project is a tribute to the legendary cryptographer Hal Finney, inspired by [his 1998 talk](https://www.youtube.com/watch?v=YjHVNstGLIQ).

It showcases a zero-knowledge proof of possession for a SHA-1 hash pre-image without revealing the pre-image itself. The proof is achieved by utilizing [this SHA-1 hash function implementation](https://github.com/michaelelliot/noir-sha1) written in [Noir](https://noir-lang.org).

## Usage

Install Noir:
```sh
curl -L https://raw.githubusercontent.com/noir-lang/noirup/main/install | bash
noirup -v 0.10.5
```

Run tests:
```sh
nargo test
```

Generate a proof using inputs in `Prover.toml`:
```sh
nargo prove
```

Verify the proof:
```sh
nargo verify
```
