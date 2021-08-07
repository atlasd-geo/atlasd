<div align="center">
  <img width="200" height="200" src="https://user-images.githubusercontent.com/79056955/128594497-46dcd431-6723-4d2f-9f68-a2fd5c569e8c.png"/>
 </div>

# Atlasd
Welcome to Atlasd! If you're new to the project, we encourage you to read all of the information below before getting started.


## Overview
Atlasd (say "at last!"; think Atlas) aims to be **web-first mapping application.** Atlasd strives to empower developers, low-code, and no-code users to create cartographic content on the web, for the web. In contrast to services like ArcGIS online and MangoMap, Atlasd intends to be free and open-source.

Grandiose aside, Atlasd is above all else supposed to a *fun* open source project. We hope folks of all skills and interests can try, fail, learn, grow, and maybe even succeed. As you read through, we hope you'll be convinced that there is something for every kind of developer, or even simply thinker, to add to this project.

## Why a mapping web application?
Generally, because a mapping web application can benefit from lots of different kinds of contributions. But, I'll take this question in two parts: why web application? and why mapping?

### Why web application?
Web applications are ubiquitous today for good reason. You can build something user-friendly quickly, you can layer on complexity progressively, and you can pull from a vast and transparent ecosystem of web technologies. For a contributor, there are seemingly endless ways to get involved in web application development as a complete N00B, a hardened vet, or anything in between:
- Commit a new component for the frontend.
- Write a performant data store for the client.
- Design a new logo.
- Build a useful microservice.
- Contribute to the documentation.
- Add a concept to the roadmap.
- Write a template generator.

Whatever it is you want to do, there's a good chance it can be used.

### Why mapping application?
Mapping applications are particularly well-positioned to benefit from the seas of skill and interest:
- Frontends need to be pretty. Hello, the design-inclined!
- Frontends need to be infromative. Hello, content-strat cats!
- Frontends are complex and need to be fast. Suh, JS playas.
- Geoprocessing operations are mathematically intricate. Tidings, ye math-enthused youths! 
- Geoprocessing operations consume lots of data. Hi, O(1) sons!
- Benefits of separation of concerns and compute are clear. Welcome to the Discothèque, Distrotechts.
- We could use some IoT drivers. Embed yourself here... wait, uh... embed your sysems here... ah, language and culture.
- We want people to actually be able to use this beast. Pull up an external doc and begin your mentation... alright, it'll get better.
- We want contributors to actually be able to contribute. Come down amongst the laypeople thou  

## Core Values
1. **Chillax:** for once, there are no deadlines. Take your time to comment and fully and formally test your code.
2. **Fail often:** nobody is grading this; nobody is writing a performance review. Just try something. If it breaks, oh well.
3. **Fish the breadth of your seas:** again, folks of all interests. There are many ways to be useful. 
4. **Play nice:** again, folks of all skills.
5. **The humanities are finally useful:** write something interesting every now and then. It makes reading this shtuff much more entertaining.


## Getting started
> The best way start is to stand.
> 
> -Santa Claus to the Winter Warlock, *Santa Claus is Coming to Town*

1. Read the rest of this document. 
2. Read the [Style Guide]().
3. Read the [Contribution Guidelines]().
4. Read the [Architecture Quickstart]().
5. Pick a repository to contribute to.
6. Read its guidelines.
7. Do its [Quick Start Activity]().
8. Idk. You tell me.

## Roadmap

## Architecture
Atlasd will rely on a **microservice-based** architecture. This is, in part, to keep the code modular and, ideally, to minimize infrastructure costs on delpoyment. But, perhaps more importantly, we hope this modular structure encourages contributors to start their own repositories and build amazing things to feed the Atlasd ecosystem.

To learn more about the overall architecture, please visit the atlasd-architecture repo.

## Repository Types
Repositories within Atlasd should generally fall into one of five categories: **clients**, **microservices**, **packages**, **utilities**, and **meta**.

### Clients
Clients are the client-side applications that tie all of the Atlasd ecosystem together. 

Work is under way on the following clients:
- [atlasd-client (Main Web Client)](https://github.com/atlasd-geo/atlasd-client)

### Microservices
Microservices are the server-side applications that enable the clients do all the cool things we need them to do. This can a least-cost path service, a geo-rectfier, an account icon uploader, an IP piggy-bank that wires money to Zuck on every call--anything really.

There are not any clients being worked on.

### Packages 
Packages are bits of reusable logic that ought not be stuck inside a single application. If for example, you write a nice Python module to compute the average distance between points on a map layer, you should probably make that package.

There are not any packages being worked on.

### Utilities
If you like making development processes run better, this is for you. Whether it's template generators, setup scripts, or whatever other best-pratice-enforced-by-code there's always a lot that can be done to help make dev easier and more standardized.

There are not any utilities being worked on.

### Meta
Meta repositories are repsitories that help provide documentation, roadmaps, and formalized opionns on Atlas development. Even if you don't feel comfortable developing, we encourage you to read and contribute to the meta.

Work is under way on the following meta:
-[atlasd-style-meta (Style Guide)]()
-[atlasd-contributions-meta (Contribution Guide)]()
-[atlasd-roadmap-meta (Project Roadmap)]()



