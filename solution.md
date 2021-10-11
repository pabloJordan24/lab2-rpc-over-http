# Web Engineering 2021-2022 / Lab2 RPC over HTTP


## How to build and run 

This section shows how to run the `server` and the `client`. 

First of all, you must be aware of something: `server` must be built and run before `client`.
If not, an error occurs because `client` needs a file published by `server`:

![alt text](https://github.com/pabloJordan24/lab2-rpc-over-http/blob/work/error.png?raw=true)

# Server

Use `./gradlew :server:build` to build the server and `./gradlew :server:bootRun` to fire it up.

# Client

Use `./gradlew :client:build` to build the client and `./gradlew :client:bootRun` to fire it up.

# Result

Screen message appearing if everything worked fine: 
```
Result of translating [hello] is [hola].
```

## Adjustments

File Server.kt was incomplete. Server was not responding client. This has been fixed by adding 
a TranslationResponse object with the matching translated text.
