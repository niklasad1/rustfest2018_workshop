# Sample project for the static analysis workshop at rustfest Paris (2018)

## Prerequisites

```bash
rustup override set nightly-2018-05-19
```

## Installing the checker

```
cargo install
```

## Running the checker

We're changing the target-dir in order to prevent rebuilding when building normally without the checker

```bash
RUSTC_WRAPPER=rustfest2018_workshop cargo check --target-dir /tmp/checker/`pwd`
```