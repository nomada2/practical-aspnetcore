# Microsoft Orleans (3)

These are simple samples to play with [Microsoft Orleans](https://github.com/dotnet/orleans), a cross-platform framework for building robust, scalable distributed applications.

This section is very early in development. My experience in using an Actor framework is ZERO. Welcome to the world of Grains and Silo.

The order to create a simple Orleans project seems to be:

- Create the Interfaces
- Create the Grains
- Create the Silo
- Create the Client

## Samples

- [Hello World](hello-world)

  This sample is a sample from Orleans that I simplify and port to C# 9. 

- [Hello World with Redis storage](hello-world-2)

  In the previous Hello World sample, once you stop the `silo`, the messages are gone. In this sample we use Redis to store the Grain between `silo` restarts so we won't lose the messages.

- [ASP.NET Core and Orleans](hello-world-3)

  Co-host Orleans and ASP.NETCore together. Everything in a single `Program.cs` file.