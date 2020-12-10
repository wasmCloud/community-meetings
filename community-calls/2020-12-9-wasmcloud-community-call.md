**<span style="text-decoration:underline;">wasmCloud Community Meeting - 2020-12-9</span>**

**<span style="text-decoration:underline;">Attendees</span>**

**<span style="text-decoration:underline;">Goal</span>**

Enable developers to build their functions and services in webassembly and run them everywhere.

**<span style="text-decoration:underline;">Introductions</span>**

*   Warren, Chris

**<span style="text-decoration:underline;">Demo</span>**



*   Wash (WAsm SHell) REPL, Brooks Townsend
    *   Goal, combine all utilities
    *   Features: signing, keys, lattice mgmt, manage capability providers
    *   
    *   REPL features
        *   View logs, change verbosity

**<span style="text-decoration:underline;">Community News</span>**



*   wasmTime community meeting is Thursday 12/10 at 1:00
    *   [Meeting Agenda](https://docs.google.com/document/d/1ZtxZNWbTNIhDdIXt27NQdwuc6D5O288l5HZKc_wC0FQ/edit#)
    *   [bytecodealliance/rfcs](https://github.com/bytecodealliance/rfcs/pulls)
*   Deis Labs
    *   [https://deislabs.io/posts/introducing-yo-wasm/](https://deislabs.io/posts/introducing-yo-wasm/)
        *   C, Rust in now
        *   Integration into Visual Studio
        *   Totally and trivial plugable
        *   Swift next maybe
        *   VS Code Debugger support
        *   Default set of actions
        *   Support for wasmCloud & wasi atm
        *   Support for github actions for pushing to containers
        *   Wapc 
            *   Yeoman would call out to wapc generator
            *   Could be a plugin for wapc compliant modules

**<span style="text-decoration:underline;">waSCC Current</span>**



*   ToDo Followup
    *   Krustlet & Crit followup, Chris & Ralph (hold? Chris out)
*   Brooks / Radu follow up on 
    *   [https://github.com/deislabs/krustlet/pull/453](https://github.com/deislabs/krustlet/pull/453)
*   Jarrod - turbulence & work

Blogpost list for community folks, Ralph, 



*   Ralph has a list of potential blogposts; will be circulating ideas and topics to write about in a rough time frame
*   List of potential blogposts:
    *   [https://hackmd.io/@y7qXqYh2SdqS3oy5XujVDA/B1Q1qISjw](https://hackmd.io/@y7qXqYh2SdqS3oy5XujVDA/B1Q1qISjw)

.15 Review



*   Kevin
    *   Still finishing up last few interfaces on control interfaces
        *   Auctions are being test & working on those
        *   Live update stuff is now in
        *   Setup some docker scripts so 
    *   Distributed cache data needs some reconsideration
        *   Do we need an actor to handle the cache here
        *   Shouldn’t be single server / central point of failure
        *   Support offline / intermittent access
        *   Short term: manage oci ← → image registry
        *   Similar to friction to k8s etcd
        *   CRDT based diffs
            *   Impact on the wire is minimal
            *   Future problem is how to host the huge caches in memory
            *   Each of the hosts; how much information it can cache
                *   Ie arudino vs. full back end cloud
        *   
*   Chris
*   Brooks
*   Bill
*   Phil
*   waPC pull request
    *   Radu
    *   Everyone is doing calling
*   What about the wasmcloud
*   ADL (Architecture Decision Log)
    *   [https://wasmcloud.github.io/adr/](https://wasmcloud.github.io/adr/)
    *   ADL for register usage
*   Demo Script for the new wasmCloud Experience:
    *   [https://docs.google.com/document/d/11QWnLiep4B3F2KOr7kYBNumgYqFVdXf6Jur_7tLTM04/edit?usp=sharing](https://docs.google.com/document/d/11QWnLiep4B3F2KOr7kYBNumgYqFVdXf6Jur_7tLTM04/edit?usp=sharing)

**<span style="text-decoration:underline;">Open PRs / Issue Review</span>**



*   [https://github.com/wasmCloud/wasmCloud/issues](https://github.com/wasmCloud/wasmCloud/issues)
*   [https://github.com/wasmCloud/wasmCloud/pulls](https://github.com/wasmCloud/wasmCloud/pulls)
*   Other components?

**<span style="text-decoration:underline;">waSCC Topic Backlog</span>**



*   Docs Rewrite
*   wasmCloud
*   Krustlet larger update
*   ADL (Architecture Decision Log)
    *   [https://wascc.github.io/adr/](https://wascc.github.io/adr/)
    *   ADL for register usage
*   Katakota Tutorials
*   Krustlet / wasm3 on small devices
    *   Constrained & JIT experience issues
*   EdX online class is January
    *   Another source of learning and documentation 
*   Yeoman / wapc generator

**<span style="text-decoration:underline;">Shared To Do:</span>**

What / Who / When



*   

**<span style="text-decoration:underline;">Post Call Feedback</span>**



*   