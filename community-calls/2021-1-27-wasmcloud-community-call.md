**<span style="text-decoration:underline;">wasmCloud Community Meeting - 2021-1-27</span>**

**<span style="text-decoration:underline;">Attendees</span>**



*   Liam Randall
*   Kevin Hoffman
*   Jarod
*   Justin
*   Andrew Brown
*   JMW
*   Andrew Brown
*   Gustaveiman
*   Bill Young
*   Christopher Marshall
*   Jordan Rash
*   Kevin Falnsburg
*   Ralph
*   Taylor Thomas
*   Matt Butcher

**<span style="text-decoration:underline;">Goal</span>**

Enable developers to build their functions and services in WebAssembly and run them everywhere.

**<span style="text-decoration:underline;">Introductions</span>**



*   John Mark Walker, Capital One Bank
*   Kevin Flansburg, Domino Data Lab

**<span style="text-decoration:underline;">Demo - </span>**



*   Brooks, Polyglot Actors with WasmCloud
    *   Leveraging wild for contracts
*   Story: write a program that can increment a KV db in response to an HTTP Request
    *   Interact with a key value database
    *   Start with write interfaces: written in wild
    *   This case:
        *   Contract is a business level contract
            *   No information about how the http request comes in
            *   No port opening, no threading
            *   Purely an abstraction around business
        *   Keyvalue contract
            *   Getting keys
            *   Retrieving keys
            *   Just abstractions around a key value interaction looks like
        *   Mention the wapc command interface
            *   From our wild we can generate language-specific interfaces for our lang
            *   Generate rust
            *   See the api being formed here
    *   The cli around the workflow
        *   https://github.com/wapc/cli
        *   wapc new assemblyscript hello_world
        *   Then use “make” to generate your interfaces
    *   Story: one loves rust, one loves assembly script
        *   Write their own competing actors
    *   Opening kv counter as rust
        *   We still don’t know where the http comes from
        *   Or what the key value store is
        *   We are just using he default “kv.default”
    *   Open kv counter as assembly script
        *   Same pattern; generic actors
        *   10 lines of code for the most part
    *   Wash up (launch an interactive repl)
        *   Ctl get hosts
        *   Ctl get inventory (see wasmcloud core running)
        *   Ctl start actor wasmcloud.azurecr.io/kv
        *   Ctl start provider redis
        *   Ctl start provider httpserver
        *   Ctl get inventory
        *   Ctl link kv counter public key & redis 
    *   Thats it, everything running in one place
        *   Curl localhost:8080 comes up
        *   If we hit 8081 - we now hit as actor
            *   Still works & continues
            *   Still linked to redis and http
    *   No dependencies on a webserver or anything else
    *   Now you can test your business logic
        *   Poke and prod actor independent of business logic

**<span style="text-decoration:underline;">Demonstration 2</span>**



*   Kevin Flansburg: Krustlet KRATOR demo: Kubernetes Rust stATe machine operatOR
*   https://github.com/deislabs/krustlet/tree/master/crates/krator
*   Kevin works on rust and kubernetes 
    *   Kurstlet now at a state machine model for defining and managing pod states in the krustlet
    *   Broke this out into a new crate
    *   Goal: improve the reliability of managing pod lifecycle
        *   Register, pull, running
    *   Split this out into it’s own crate
        *   Now you can write more generic operators 
    *   Crate krater
        *   Operator trait you implement
        *   Primarily the kubernetes resource type
        *   Leverage k8s open api types
        *   Can describe your own types, state of your objects internally
        *   Supply initial state & deleted state
            *   Can automatically transition to that state
            *   1 status, gets sent to kubernetes api
        *   

**Community Activity**



*   CFP: [https://events.linuxfoundation.org/cloud-native-wasm-day/](https://events.linuxfoundation.org/cloud-native-wasm-day/)
*   [https://webassembly-summit.org/](https://webassembly-summit.org/)
*   wasmTime (Thursday’s 1:00
*   Run time working group

**wasmCloud Deployment Options**



*   Via wasmCloud packages
*   Krustlet is another existing deployment option
    *   [https://github.com/deislabs/krustlet/blob/master/docs/howto/README.md](https://github.com/deislabs/krustlet/blob/master/docs/howto/README.md)
*   Krustlet on GKE
    *   https://github.com/deislabs/krustlet/blob/master/docs/howto/krustlet-on-gke.md
*   Lambda
*   Go runtime in a terraform provider
    *   [https://github.com/EvilSuperstars/terraform-provider-wapc](https://github.com/EvilSuperstars/terraform-provider-wapc)
*   Custom \


**<span style="text-decoration:underline;">Community News</span>**



*   wasmTime community meeting is postponed this week, Thursday 1/21/2020 at 1:00
    *   [Meeting Agenda](https://docs.google.com/document/d/1ZtxZNWbTNIhDdIXt27NQdwuc6D5O288l5HZKc_wC0FQ/edit#)
*   https://events.linuxfoundation.org/cloud-native-wasm-day/

**<span style="text-decoration:underline;">wasmCloud Current</span>**



*   Reminder: Azure Registry Complete
    *   enable public anonymous pull (downloads) on azure container register.
    *   [Wasmcloud.azurecr.io](http://wasmcloud.azurecr.io/) configured for public
*   wasmCloud site update progress
*   [Actor-interfaces](https://github.com/wasmCloud/actor-interfaces/issues)
*   [Wash REPL](https://github.com/wasmCloud/wash/issues)
*   Krustlet, cut to new release (hold till release)
    *   Need to move the provider over to repo
    *   Then cut it over 
    *   Lot’s in flight - kube, tokyo, etc
*   

**<span style="text-decoration:underline;">RELEASE TARGET: Jan 31, 2021 WASMCLOUD .15</span>**



*   Demo Script Updates for the new wasmCloud Experience:
    *   [https://docs.google.com/document/d/11QWnLiep4B3F2KOr7kYBNumgYqFVdXf6Jur_7tLTM04/edit?usp=sharing](https://docs.google.com/document/d/11QWnLiep4B3F2KOr7kYBNumgYqFVdXf6Jur_7tLTM04/edit?usp=sharing)

**<span style="text-decoration:underline;">Open PRs / Issue Review</span>**



*   [https://github.com/wasmCloud/wasmCloud/issues](https://github.com/wasmCloud/wasmCloud/issues)
*   [https://github.com/wasmCloud/wasmCloud/pulls](https://github.com/wasmCloud/wasmCloud/pulls)
*   ADL (Architecture Decision Log)
    *   [https://wasmcloud.github.io/adr/](https://wasmcloud.github.io/adr/)

Help Wanted:



*   Remove git dependencies
*   Actor interfaces for wasmCloud
*   Documentation
*   .2 milestone requests for wash

**<span style="text-decoration:underline;">wasmCloud Topic Backlog</span>**



*   2020-1-13
    *   Demo: WIDL, Phil Kedy
    *   Demo: waPC, Phil Kedy
    *   Demo: waPC cli, Phil Kedy
*   2020-1-20
    *   Bindle
    *   https://github.com/deislabs/bindle/
*   Demo: Code gen + API easier to use
    *   [https://github.com/wasmcloud/actor-interfaces](https://github.com/wasmcloud/actor-interfaces)
    *   Need Go & Assembly Script
    *   
*   Docs Rewrite
*   Critical Stack + krustlet
*   wasmCloud
*   Krustlet larger update
*   ADL (Architecture Decision Log)
    *   [https://wasmcloud.github.io/adr/](https://wasmcloud.github.io/adr/) 
    *   ADL for register usage
*   Katakota Tutorials
*   Krustlet / wasm3 on small devices
    *   Constrained & JIT experience issues
*   EdX online class is January
    *   Another source of learning and documentation 
*   Yeoman / wapc generator
    *   Ivan 
    *   After 1 pm pacific

**<span style="text-decoration:underline;">Shared To Do:</span>**

What / Who / When
