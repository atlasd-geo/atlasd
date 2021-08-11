# Architecture Quickstart
Atlasd relies on a microservice architecture. If you aren't familiar with microservice architectures, check out this article from [Microsoft Azure](https://docs.microsoft.com/en-us/azure/architecture/guide/architecture-styles/microservices).

The choice to use a microservice architecture was made, in part, to keep the code modular and, ideally, to minimize infrastructure costs on delpoyment. But, perhaps more importantly, we hope this structure encourages contributors to start their own repositories and build amazing things to feed the Atlasd ecosystem.

You do not need to fully, or even remotely, understand the architecture to begin contributing. However, if you are interested in creating a repo of your own, demonstrated understanding of the architecture is necessary.

## Philosophy
While certain hosting services may be suggested, *see* [Contribution Guidelines](https://github.com/atlasd-geo/atlasd/blob/main/Contribution%20Guidelines.md), we encourage all software to be written largely machine and service independent. Containerization and separation of concerns should be adhered to consistently. 

## Services
The service structure of Atlasd will include the following:
- Client delivery services
- Identity provider
- Role provider
- Central database
- Microservices
- File service

The **identity provider** and **role provider** together form the Auth system that should used by all other services. Auth0 has been proposed for the identity provider and Fauna has been proposed as the BAAS that will enable the implementation of a role provider. Ideally, the role provider and central database will exist as one service; any data that should be accessible throughout the application ought to live in the same place as roles, as they too should be accesible throughout the application.

For a visual representation of the service architecture, review the [Architecture Quickstart](https://docs.google.com/presentation/d/1X_PXxBQBLjXTfP17kSLM6m6KB487YMzLb4R2CXMUzfE/edit?usp=sharing) slide deck.

![Screen Shot 2021-08-07 at 2 23 44 PM](https://user-images.githubusercontent.com/79056955/128614182-480204e8-5bbe-4991-81be-80443c823298.png)


## Repository Types
Due to the above architecture, repositories within Atlasd should generally fall into one of five categories: clients, microservices, packages, utilities, and meta.

### Clients
Clients are the client-side applications that tie all of the Atlasd ecosystem together.

Work is under way on the following clients:

[atlasd-client (Main Web Client)](https://github.com/atlasd-geo/atlasd-client)

### Microservices
Microservices are the server-side applications that enable the clients do all the cool things we need them to do. This can a least-cost path service, a geo-rectfier, an account icon uploader, an IP piggy-bank that wires money to Zuck on every call--anything really.

There are not any microservices being worked on.

### Packages
Packages are bits of reusable logic that ought not be stuck inside a single application. If for example, you write a nice Python module to compute the average distance between points on a map layer, you should probably make that package.

There are not any packages being worked on.

### Utilities
If you like making development processes run better, this is for you. Whether it's template generators, setup scripts, or whatever other best-pratice-enforced-by-code there's always a lot that can be done to help make dev easier and more standardized.

There are not any utilities being worked on.

### Meta
Meta repositories are repsitories that help provide documentation, roadmaps, and formalized opinions on Atlas development. Even if you don't feel comfortable developing, we encourage you to read and contribute to the meta.

Right now the [atlasd (Main Parent Repo)](https://github.com/atlasd-geo/atlasd) is the only meta.

## Next Steps
If you're coming here on your first trip into the Atlasd project, the next place you'll want to go is [Contribution Guidelines](https://github.com/atlasd-geo/atlasd/blob/main/Contribution%20Guidelines.md).
