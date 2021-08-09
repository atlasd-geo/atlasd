# Contribution Guidelines
Getting well enough oriented to contribute to an open source project can be challenging. 
- If this is your first time here, we recommend searching [Issues](https://github.com/atlasd-geo/atlasd/issues?q=is%3Aopen+is%3Atoycontribution+) for the toycontribution tag. 
- The toycontribution tag marks activities designed to help get you started. 
- Once you've completed one, come back here to dive in.

## Issues
Issues can be assigned the labels below. If you make a new repo, please copy these all of these labels except for `toycontribution`; `toycontribution` is reserved for the Atlasd Parent Repo.

#### `no code`
Use to mark an issue that can be potentially be resolved without any code.

#### `documentation`
Use to mark any issue that is related to documentation.

#### `proposal`
Use to propose changes to process or code.

#### `enhancement`
Use to mark proposals that have been agreed are an improvement on process or code.

#### `help wanted`
Use to mark issues that need more people to resolve.

#### `question`
Use to mark general questions.

#### `duplicate`
Use to mark a duplicate before closing.

#### `toycontribution`
Use to mark an activity intended to help first time users get started.

#### `good first issue`
Use to mark an issue that doesn't require significant knowledge of process or code, but which is intended for actual use.

#### `easy`
Use to mark an issue that should be resolved easily.

#### `medium` 
Use to mark an issue that should be moderately challenging to resolve.

#### `hard`
Use to mark an issue that should be hard to resolve.

#### `ultra`
Use to mark an issue that would be a big undertaking. Big ideas and requests are suited for the ultra tag.

#### `mega`
Use to mark an issue that would be a massive undertaking. Not only should these be big ideas, but big ideas that require deep knowledge that goes beyond that commonly used in day-to-day development.

#### `bug`
Use to mark a bug in process or code.

## Repository Requirements
We expect every repository in this project to adhere to the following. If you are unclear about any of the below, please review [atlasd-client](https://github.com/atlasd-geo/atlasd-client) as an example repository.

### Utilities
The following utilities must be included with the repository.
1. **CLI to run the application**
2. **CLI to run test suites**
3. **Documentation application**
4. **Dockerfile or other means of containerization** 

### Contributing
Each repository must contain its own contributing file. Use a [Contributing.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) as a template if you are unclear where to begin.

### README
The README file for every repository should contain the following:
1. A `Run` section, describing how to run the software.
2. A `Test` section, describing how to run the test suites.
3. A `Docs` section, describing how to run the documentation application.
4. A `Container` section, describing how to run a containerized version of the software.
5. A `Quick Start Activity` describing the an activity users should use to get familiar with the project.
6. A link to the `Contributing `file.


## Git Workflow
We encourage [CI](https://www.youtube.com/watch?v=Xl62gQpAl1w) under the following parameters.

### Branches
All repositories in this project should keep branches to a minimum. We encourage the use of only `main` and `dev` branches for main repos. `main` should be used for stable release, `dev` should be used for all else. PRs should be submitted to `dev`. The use of feature branches is encouraged for individual workflows, but utlimately feature branches should not be added to the repositories on GitHub.

### Review of PRs
Contributors in a position to review PRs, should abide by the following rules:
1. **Duty to Respond:** As long as the PR is not completely irrelevant, we urge you to issue a response.
2. **Strict Merging:** Never merge a pull request that does not pass all tests. 
3. **Response by Resolution:** If the solution to a faulty PR is trivial, feel empowered to make the changes yourself. But, do let the contributor know what you changed.

## Recommended Tools and Technologies
We contributing to an existing repository or starting a new one, you ultimately have to pick the right tool for the job. That said, we recommend selecting from the tools and technologies below. If you do use the below, please adhere to any provided style guides. 

Further recommendations may be specified in documentation associated with each of the tools.

### Text Editors
[**VSCode**](https://code.visualstudio.com/)
- Tools and Best Practices: WIP.

### General Purpose Languages
[**TypeScript**](https://www.typescriptlang.org/)
- Use of plain Javascript is discouraged.
- Suggested for use with [React.js](https://reactjs.org/) frontends and [Express.js](https://expressjs.com/) backends.
- [Style Guide](https://github.com/atlasd-geo/atlasd/tree/main/languages/Typescript) 
- [With React](https://github.com/atlasd-geo/atlasd/tree/main/languages/Typescript/With%20React)

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
- [TypeScript With React](https://github.com/atlasd-geo/atlasd/tree/main/languages/Typescript/With%20React)

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

### Hosting Services
- WIP
