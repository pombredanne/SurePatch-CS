# SurePatch-CS
SurePatch Component Server.
This is a solution for transferring algorithms of software components versions processing to a external server.
In this case, the program on the user's computer (CLI App) collects reports from the operating system and package managers, generates files and uploads them to a specific external server on the global network. There they are processed, checked and parsed. The result of this operation of the server - is a set of components and versions, that are sent to the main application, accompanied by parameters for authorization of the user and are implemented into its main account.
The dedicated external server is built on multi-threaded asynchronous technology with non-blocking connections.
This approach will allow to unload the application, remove duplication of program code, define a single entry point for personal software clients and for integration with external applications such as githab, bitbaket, etc.
In addition, the client application will be reworked as an operating system service that allows monitoring changes in batch files and performing automated creation of component sets with an assessment of the dynamics of vulnerability changes on the client software.
