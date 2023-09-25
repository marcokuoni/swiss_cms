# Secure and Fast Swiss CMS
!! This is still a draft !!

## Introduction
Community driven project to create a secure and fast Swiss CMS. With following key features build into the kernel and design:
* [Sustainability](https://w3c.github.io/sustyweb)
* [Security](documents/specifications/security.md)
* Speed
* Scalability (Portability)
* Accessability
* Testing
* Documentation
* Schooling
* [User Experience](documents/specifications/user_experience.md)

Open Source and community driven. Every code can be reviewed, issued and contributed. But just reviewed code comes in the core.

### Vision
* Should be the API to the business of privates/companies (internal, partner, public)
* Data warehouse and source of truth in the core
* Easy connect to you data and send your data. With the idea to have the data decentralized at the owner of the data but connected to everyone. Always be the owner, have the control and a secure channel.
* No code low code possabilities, create a datasafe on the fly
* Education whats going on under the hood (What means to share, read only and so on. In a way everybody understands)
* Schooling for structering data and sensibilisation for data security and data privacy
* Possability to easy present content in coporate design
* Inline editing for pages
* Swiss law contracts and reconnaissance included in the system
* Good software design with package managements. But only proofed packages can be installed
* Be prepared to deploy on every plattform (Internet Computer, Cloud, OnPremise, Edge, IoT, Mobile, Desktop, Server, ...)

## Stack
### Webassembly Runtimes
* Dockerize with [WasmEdge](https://github.com/WasmEdge/WasmEdge)
  * [Docker Quickstart](https://wasmedge.org/docs/start/getting-started/quick_start_docker/)
  * [WASM Docker](https://docs.docker.com/desktop/wasm/)

#### Alternative Runtimes
* [Wasmer](https://wasmer.io/)
* [Wasmtime](https://wasmtime.dev/)


### Application Stack
* Client/Server [Leptos](https://www.leptos.dev/)

#### Alternative Application Stack
* Server [Actix](https://actix.rs/)
* Client [Yew](https://yew.rs/)

### Filehandling
Run on WASM-Container?
* [SeaweedFS](https://seaweedfs.github.io/)

### Database
Run on WASM-Container?
* [ScyllaDB](https://www.scylladb.com/)
    * https://www.scylladb.com/tech-talk/scylladb-embraces-wasm/

## Roadmap
1. develop an easy application to proof the stack
   1. Start with Leptos and deploy it through Docker by using WasmEdge
   2. Create a GUI to read and write into Database and Filesystem
   3. Create a ScyllaDB Database and deploy it through Docker (by using WasmEdge)
   4. Create a SeaweedFS Filesystem and deploy it through Docker (by using WasmEdge)
   5. Analyse and write an writeup
      * Webassembly Serverside
      * Webassembly Clientside
      * Speed
      * Security
      * Portability
      * Scalling

2. Start creating proposal to build a community for a new Webassembly CMS in relation of the vision and the first roadmap point

## Code of Conduct
* [Berlin Code of Conduct](https://berlincodeofconduct.org/)

## License
* [MIT](https://mit-license.org/)