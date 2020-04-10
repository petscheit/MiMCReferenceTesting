## MiMCSponge Reference implementation for testing
### Instruction for running:
- install dependencies globally with ```npm install -g snarkjs circom```
- switch comment at the end of mimcsponge.circom to switch between mimcFeistel and mimcSponge

### Run the following:
- compile with ```circom mimcsponge.circom --r1cs --sym --wasm```
- setup with ```snarkjs setup -r mimcsponge.r1cs```
- compute witness with ```snarkjs calculatewitness --wasm mimcsponge.wasm --input input.json --witness witness.json```
- get proof ```snarkjs proof```
- after running this outputs can be found in public.json