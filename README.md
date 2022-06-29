# protobuf

A protocol buffer is a data serialization mechanism.

This repo contains example from: https://developers.google.com/protocol-buffers/docs/pythontutorial

### Key points
- The serialized data is in binary format
- A schema `.proto` file is required
- Code to use the schema has to be generated for the specific language.

### How to use
- first you have to create a `.proto` file describing the schema
- use the `protoc` compiler to generate language specific clases, 
	for example `protoc -I=. --python_out=. myfile.proto` to generate python classes
- use the generated code with your code to read and write data using the schemas defined by the protobuf

