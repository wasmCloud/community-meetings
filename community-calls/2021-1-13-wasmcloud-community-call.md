**<span style="text-decoration:underline;">wasmCloud Community Meeting - 2021-1-13</span>**

**<span style="text-decoration:underline;">Attendees</span>**

**<span style="text-decoration:underline;">Goal</span>**

Enable developers to build their functions and services in webassembly and run them everywhere.

**<span style="text-decoration:underline;">Introductions</span>**

**<span style="text-decoration:underline;">Demo</span>**



*   Next Demo: 2021-1-20 Phil Kedy: WIDL 
*   Today: [wapc cli](https://github.com/wapc/cli)
    *    \


**<span style="text-decoration:underline;">Community News</span>**



*   wasmTime community meeting is Thursday 1/21/2020 at 1:00
    *   [Meeting Agenda](https://docs.google.com/document/d/1ZtxZNWbTNIhDdIXt27NQdwuc6D5O288l5HZKc_wC0FQ/edit#)

**<span style="text-decoration:underline;">wasmCloud Current</span>**



*   Remidner: Azure Registry Complete
    *   enable public anonymous pull (downloads) on azure container register.
    *   [Wasmcloud.azurecr.io](http://wasmcloud.azurecr.io/) configured for public
*   wasmCloud site update progress
*   [Actor-interfaces](https://github.com/wasmCloud/actor-interfaces/issues)
*   [Wash REPL](https://github.com/wasmCloud/wash/issues)
*   Krustlet, cut to new release (hold till release)

Review - .15 open tickets



*   Remaining To do on .15
    *   Packaging
        *   Home Brew
            *   Current manual process
            *   The checksum and release is manual
        *   Arm type packages
            *   
    *   Automation for builds on wasmCloud repo
        *   
    *   Azure Registry
        *   wasmCloud
*   Demo Script Updates for the new wasmCloud Experience:
    *   [https://docs.google.com/document/d/11QWnLiep4B3F2KOr7kYBNumgYqFVdXf6Jur_7tLTM04/edit?usp=sharing](https://docs.google.com/document/d/11QWnLiep4B3F2KOr7kYBNumgYqFVdXf6Jur_7tLTM04/edit?usp=sharing)

**<span style="text-decoration:underline;">Open PRs / Issue Review</span>**



*   [https://github.com/wasmCloud/wasmCloud/issues](https://github.com/wasmCloud/wasmCloud/issues)
*   [https://github.com/wasmCloud/wasmCloud/pulls](https://github.com/wasmCloud/wasmCloud/pulls)
*   ADL (Architecture Decision Log)
    *   [https://wasmcloud.github.io/adr/](https://wasmcloud.github.io/adr/)
*   

**<span style="text-decoration:underline;">waSCC Topic Backlog</span>**



*   2020-1-13
    *   Demo: WIDL, Phil Kedy
    *   Demo: waPC, Phil Kedy
*   2020-1-20
    *   Bindle
    *   https://github.com/deislabs/bindle/
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