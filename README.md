## Foundry code-examples

### Project structure

`lib` has libraries such as [https://onbjerg.github.io/foundry-book/reference/ds-test.html](ds-test) and @openzeppelin, you can import libraries from here via remappings in `foundry.toml`.

`remappings = ['ds-test/=lib/ds-test/src/']`

`src` has the tests the developer will write (and will run upon writing `forge test`). `src` also has your contracts which will be compiled via `forge build`.

```
├── foundry.toml
├── lib
│   └── ds-test
│       ├── LICENSE
│       ├── Makefile
│       ├── default.nix
│       ├── demo
│       └── src
├── out
│   ├── Contract.sol
│   │   └── HelloWorld.json
│   ├── Contract.t.sol
│   │   ├── ContractTest.json
│   │   └── HelloWorldTest.json
│   └── test.sol
│       └── DSTest.json
└── src
    ├── Contract.sol
    └── test
        └── Contract.t.sol
```

### Branches
1. hello-world: Simple hello world program with a sample test