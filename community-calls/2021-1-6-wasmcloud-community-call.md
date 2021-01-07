**<span style="text-decoration:underline;">DRAFT wasmCloud Community Meeting - 2021-1-6</span>**

**<span style="text-decoration:underline;">Attendees</span>**

**<span style="text-decoration:underline;">Goal</span>**

Enable developers to build their functions and services in webassembly and run them everywhere.

**<span style="text-decoration:underline;">Introductions</span>**



*   Milan Bhatia, Capital One
    *   POC using wasm tools
*   Felix, Shopify automation group
    *   Wasm to run low latency scripts
*   Jeff Charles, Shopify automation group
    *   Building a product, model

**<span style="text-decoration:underline;">Demo</span>**



*    2020-1-13 Phil Kedy
    *   Demo: WIDL
    *   Demo: waPC
*   Today: wasi-nn
    *   Work out of intel driving portability of models
    *   Enable access to dedicated hardware
    *   Great block diagram
        *   Currently enables OpenVINO
        *   Wasmtime implements wasi-nn

![alt_text](images/2021-1-6-wwasi-nn.png "wasi-nn background")

    *   In wasmtime example
        *   Has enabled alexnet example to run open vino
        *   Compiles example file into wasm
        *   Requires use of feature `"flag --features wasi-nn"`
    *   Demo
        *   Loading is slow atm, stuff to sort out in wasi
        *   Finds the pizza
    *   For more information:
        *   [https://bytecodealliance.org/articles/implementing-wasi-nn-in-wasmtime](https://bytecodealliance.org/articles/implementing-wasi-nn-in-wasmtime)
        *   [https://bytecodealliance.org/articles/using-wasi-nn-in-wasmtime](https://bytecodealliance.org/articles/using-wasi-nn-in-wasmtime)
    *   What about other engines
        *   It’s early in a few ways - wasi is early.  Fundamentals needs to be sorted out (networking, file, etc).  Approach was to look ahead where there is down the road.
        *   This is about getting feedback on the initial concept.
        *   Maybe switch to a model builder api - control the nodes in the graph through wasi
    *   Other implementations
        *   Tensorflow using wasi-nn
        *   What changes would they need to use this in production
    *   Tensorflow for example
        *   Working closely with the web-nnn group
        *   Collection of top ml practitioners
        *   This is the nexus of research, design, etc
        *   Similar proposal for model loader in that community
        *   One driving factor to do this is the performance difference between native & wasm ---> the gap is pretty big
        *   Discussing SIMD for example (128 bit) but in cpu world & gpu (512) is the standard
    *   Feedback and engagement
        *   Will respond to issues in wasi-nn or wasmtime
        *   If you want to discuss, he’s on zulip all the time
        *    \


**<span style="text-decoration:underline;">Community News</span>**



*   wasmTime community meeting is Thursday 1/7/2020 at 1:00
    *   [Meeting Agenda](https://docs.google.com/document/d/1ZtxZNWbTNIhDdIXt27NQdwuc6D5O288l5HZKc_wC0FQ/edit#)

**<span style="text-decoration:underline;">wasmCloud Current</span>**



*   ToDo Followup
    *   Krustlet & Crit followup, Chris & Ralph (hold? Chris out)
*   Azure Registry Complete
    *   enable public anonymous pull (downloads) on azure container register.
    *   [Wasmcloud.azurecr.io](http://wasmcloud.azurecr.io/) configured for public
*   wasmCloud site update progress
*   Blogpost list for community folks, Ralph, 
    *   Ralph has a list of potential blogposts; will be circulating ideas and topics to write about in a rough time frame
    *   List of potential blogposts:
        *   [https://hackmd.io/@y7qXqYh2SdqS3oy5XujVDA/B1Q1qISjw](https://hackmd.io/@y7qXqYh2SdqS3oy5XujVDA/B1Q1qISjw)

Review - .15 open tickets



*   Remaining To do on .15
    *   [Actor-interfaces](https://github.com/wasmCloud/actor-interfaces/issues)
        *   4 Rust
        *   7 Go
        *   7 Assembly Script
    *   Wash up / REPL
    *   Packaging
        *   Home Brew
            *   Current manual process
            *   The checksum and release is manual
        *   Arm type packages
            *   Looking at arm64
            *   Done this for wasm3 provider for krustlet
            *   On the linux host for the ci instance
            *   Had to have the entire c compiler, cross compiled for arm
            *   The c compiler, c lang, to compile tino llvm
                *   Can happen on amd64
                *   Works but if you have to deal with openssl you have to compile that from scratch
                *   It really depends on dependencies
                *   Not truly scalable
                *   Example Artisinal recipe for building for arm64 on x86:
                *   [https://github.com/deislabs/krustlet/blob/9de974a5ee8c21a9f8284fe6ef7a444e25cdafc0/.github/workflows/build.yml#L78](https://github.com/deislabs/krustlet/blob/9de974a5ee8c21a9f8284fe6ef7a444e25cdafc0/.github/workflows/build.yml#L78)
    *   Automation for builds on wasmCloud repo
        *   Don’t have automated testing on repo
        *   Need the action step
    *   Azure Registry
        *   wasmCloud
*   Demo Script Updates for the new wasmCloud Experience:
    *   [https://docs.google.com/document/d/11QWnLiep4B3F2KOr7kYBNumgYqFVdXf6Jur_7tLTM04/edit?usp=sharing](https://docs.google.com/document/d/11QWnLiep4B3F2KOr7kYBNumgYqFVdXf6Jur_7tLTM04/edit?usp=sharing)
*   Bindle release
    *   [https://github.com/deislabs/bindle/](https://github.com/deislabs/bindle/)
*   Krustlet will be cutting over to wasmCloud in new release
    *   End of month, moving it over
    *   Code commit
    *   New release on the way; updating api endpoints
    *   wasmCloud has a similar thing
    *   On our list to explore
    *   Take a look at replacing pr files (provider archives) with bindle’s
    *   Thinking through security model & signing things; people give it a try, etc

**<span style="text-decoration:underline;">Open PRs / Issue Review</span>**



*   [https://github.com/wasmCloud/wasmCloud/issues](https://github.com/wasmCloud/wasmCloud/issues)
*   [https://github.com/wasmCloud/wasmCloud/pulls](https://github.com/wasmCloud/wasmCloud/pulls)
*   ADL (Architecture Decision Log)
    *   [https://wasmcloud.github.io/adr/](https://wasmcloud.github.io/adr/)
*   

**<span style="text-decoration:underline;">waSCC Topic Backlog</span>**



*   2020-1-6
    *   Demo: wasi-nn Demo, Andrew Brown
*   2020-1-13
    *   Demo: WIDL, Phil Kedy
    *   Demo: waPC, Phil Kedy
*   2020-1-20
    *   Bindle
*   Demo: Code gen + API easier to use
    *   [https://github.com/wasmcloud/actor-interfaces](https://github.com/wasmcloud/actor-interfaces)
    *   Need Go & Assembly Script
    *   
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

Discusion



*   Why did wasmCloud use wasm3 by default?
    *   Why jit vs. 
*   We should call to action and test with wasmTime and not just default wasm3
*   Should we have an experimental branch
    *   To see how they work together
*   Other features
    *   Wasm simd for example
    *   Wasmtime has it, do other engines like wasm3?
    *   That feature is less esoteric than wasi-nn