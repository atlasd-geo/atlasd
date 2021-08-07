# Contribution Guidelines
Follow these guidelines when contributing to the Atlasd project.

## Contributing
Each repository should provide its own Contributing.md. If you are creating a repo and don't have one in mind, we suggest reviewing this template: [Contributing](https://gist.github.com/PurpleBooth/b24679402957c63ec426).

## Git Workflow
We encourage [CI](https://www.youtube.com/watch?v=Xl62gQpAl1w) under the following parameters.

### Branches
All repositories in this project should keep branches to a minimum. We encourage the use of only `main` and `dev` branches for main repos. `main` should be used for stable release, `dev` should be used for all else. PRs should be submitted to `dev`. The use of feature branches is encouraged for individual workflows, but utlimately feature branches should not be added to the repositories on GitHub.

### Review of PRs
For more on review of PRs see Review.

## Repository Requirements
We expect every repository in this project to adhere to the following
- Expose a CLI to run the application.
- Expose a CLI to run test suites.
- Provide a documentation server.
- Provide a working Dockerfile or other containerization. 

Information about working with each of these utilities must provided under the headers Run, Test, Docs, and Container in the repository README.md. For a template README.md, see README_TEMPLATE. 

If you are unclear about any of the above, please review [atlasd-client](https://github.com/atlasd-geo/atlasd-client) as an example repository.

## Recommended Tools and Technologies
We contributing to an existing repository or starting a new one, you ultimately have to pick the right tool for the job. That said, we recommend selecting from the tools and technologies below. If you do use the below, please adhere to any provided style guides.

### Text Editors
[**VSCode**](https://code.visualstudio.com/)
- Tools and Best Practices: WIP.

### General Purpose Languages
[**Typesrcipt**](https://www.typescriptlang.org/)
- Use of plain Javascript is discouraged.
- Suggested for use with [React.js](https://reactjs.org/) frontends and [Express.js](https://expressjs.com/) backends.
- Style Guide 

[**Python**](https://www.python.org/)
- Use for backend development.
- Style Guide: WIP.

[**Haskell**](https://www.haskell.org/)
- Use for backend development, particularly with highly concurrent systems.
- Use to target [WebAssembly](https://webassembly.org/) for high performance frontend components.
- Style Guide: WIP.

[**Rust**](https://www.rust-lang.org/)
- Use for backend development.
- Style Guide: WIP.

[**C++**](https://www.cplusplus.com/)
- Use for backend development.
- Use to target [WebAssembly](https://webassembly.org/) for high performance frontend components.
- Style Guide: WIP.

### Frontend Technologies
[**React/React Native**](https://reactjs.org/)
- Use for most frontend development.
- Style Guide

[**Electron**](https://www.electronjs.org/)
- Use with React for any desktop application development.

[**WebAssembly**](https://webassembly.org/)
- Use for experimentation with high-performance features.
- Use with Haskell or C++.

### Backend Technologies
[**Node.js**](https://nodejs.org/en/)
- Use for general purpose backend.

[**Express.js**](https://expressjs.com/)
- Use with Node.js for general purpose backend.

[**Flask**](https://flask.palletsprojects.com/en/2.0.x/)
- Use for general purpose backend.

[**Fast API**](https://fastapi.tiangolo.com/)
- Use for general purpose backend.

[**Yesod**](https://www.yesodweb.com/)
- Use for highly concurrent backends (or if you want functional street cred).

[**Rocket**](https://rocket.rs/)
- Use for general purpose backend.

[**CppCMS**](http://cppcms.com/wikipp/en/page/main)
- Use for high-performance backend.

### Data
[**Fauna**](https://docs.fauna.com/fauna/current/)
- Go to BAAS.
- FQL is great!

[**RabbitMQ**](https://www.rabbitmq.com/)
- Go to message broker.

[**Redis**](https://redis.io/)
- Alternative message broker.

[**MQTT**](https://mqtt.org/)
- IoT message broker.

[**MongoDB**](https://www.mongodb.com/)
- Use whenever a database distinct from the central DB is necessary.

### Auth
[**Auth0**](https://auth0.com/)
- Go to SSO and identity provider.



