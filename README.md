# WAGI-On-Lambda-Edge
Write `Grain` code, compile it to `WASM`, turn it into http handler with `WAGI`, and then deploy it to `AWS Lambda@Edge`. Working in process.

## Setup
1. Grain
2. WAGI
3. (Optional) Wasmer

## Run (HTTP X)

```shell
grain compile hello.gr
```

```shell
# wasmer hello.gr.wasm args --env [key]=[value]
wasmer hello.gr.wasm
```

Or you can combine compile & run like below :

```shell
grain hello.gr
```

## Run (HTTP O)
```shell
wagi -c modules.toml
curl localhost:3000/hello?hello=world
```
## Deploy to Lambda@edge
To be added...
