# jito-ts
Welcome to the Jito Typescript SDK repository! Use this to interact with the block-engine, relayer and future Jito APIs.

## Building Protos
The generated proto files have been committed for convenience, but if there's ever a change you'll need to re-generate.
Steps to regenerate:
* Make sure you have protoc installed on your system
* If any new `.proto` files were added, update the `./scripts/generate-protos` script to include it.
* Run `yarn gen ${PATH_TO_PROTOS}` and commit!

**Note:** Mac users may run into an error to the effect of "protoc-gen-js: program not found or is not executable";
if this is thrown, run:
* `brew install protobuf@3`
* `brew link --overwrite protobuf@3`
* `yarn gen ${PATH_TO_PROTOS}`

