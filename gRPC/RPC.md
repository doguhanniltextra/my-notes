Remote Procedure Call is a protocol and communication mechanism that allows a computer program to execute a subroutine or procedure in a different address space (usually on another computer over a network) without the programmer explicitly coding the details for the remote interaction.

How RPC Works

1. Client Call: The client application calls a local procedure (the client sub)
2. Marshalling (Client Sub): The stub packs the function parameters into a message (serialization) suitable for transmission over the network
3. Transmission: The operating system send the message to the remote server
4. Unmarshalling (Server Stub): The server-side stub receives the message, unpacks the data (deserialization), and converts it into a format the server can process.
5. Execution and Response: The server executes the actual function and send the result back through a similar process.