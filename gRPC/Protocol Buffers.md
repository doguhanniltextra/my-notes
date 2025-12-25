Protocol buffers are a language-neutral, platform-neutral extensible mechanism for serializing structured data.

It's like JSON, except it's smaller and faster, and it generates native language bindings. You define how you want your data to be structured once, then you can use special generated source code to easily write and read your structured data to and from a variety of data streams and using a variety of languages.

### What Problems Do Protocol Buffers Solve?

Protocol buffers provide a serialization format for packets of typed, structured data that are up to a few MB in size. The format is suitable for both ephemeral network traffic and long-term data storage. Protocol buffers can e extended with new information without invalidating existing data or requiring code to be updated.

## How do Protocol Buffers Work?

- Create .proto file to define data structure
- Generate code using the protoc compiler
- Compile PB code with your project code
- Use PB classes to serialize, share and deserialize data