# LSP Multi Server Example

A language server example that demonstrates how to start a server per workspace folder. If the workspace has nested workspace folders only a server for the outer most workspace folder is started assuming that the language service handles nested code.

The example uses proposed Language Server protocol. So the code demoed here might change when the final version of the configuration and workspace folder protocol is released.

## Running the Sample

- run `npm install` in this folder. This installs all necessary npm modules in both the client and server folder
- open VS Code on this folder.
- Press Ctrl+Shift+B to compile the client and server
- Switch to the Debug viewlet
- Select `Launch Client` from the drop down
- Run the lauch config
- If you want to debug the server as well use the launch configuration `Attach to Server`


## How to Disable TypeScript for JavaScript
```json
"javascript.validate.enable": false,
"javascript.format.enable": true,
```



## Related ISSUES as of Aug 2020


The following issue points out that TypeScript will probally stay Infinit InCompatible without this rollup-languages-server as it is a Design Decission that i do not agree with i Created this project to Create a TypeScript Drop In Replacement that also improves Analyses of ECMAScript / Javascript without TypeScript.

- https://github.com/microsoft/TypeScript/issues/35589
Other Realted issues

- https://github.com/microsoft/TypeScript/pull/39840#issuecomment-671223595
- https://github.com/microsoft/TypeScript/issues/39971
- https://github.com/microsoft/TypeScript/issues/39012
- https://github.com/microsoft/TypeScript/issues/38729