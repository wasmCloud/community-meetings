
**<span style="text-decoration:underline;">waSCC Community Meeting - 2020-11-25</span>**

**<span style="text-decoration:underline;">Attendees</span>**

Kevin Hoffman

Bill Young

Shane O’Donnell

Phil Kedy

Liam Randall

**<span style="text-decoration:underline;">Goal</span>**

Enable developers to build their functions and services in webassembly and run them everywhere.

**<span style="text-decoration:underline;">Introductions</span>**



*   Shane O’Donnell, Solo.io

**<span style="text-decoration:underline;">Community News</span>**



*   wasmTime Meeting for Thursday 2020-11-26 cancelled

**<span style="text-decoration:underline;">waSCC Current</span>**



*   ToDo Followup
    *   Krustlet & Crit followup, Chris & Ralph (hold? Chris out)
    *   Blogpost list for community folks, Ralph, 
*   Microsoft scheduling conflict
*   [Architectural Decision Record](https://github.com/wascc/adr/blob/gh-pages/index.md)
    *   004 Review
*   .15 Review
    *   Kevin
        *   Main rewrite of core engine for wasmCloud is complete
        *   95% feature complete… last 95% will take a while
        *   Lattice-rpc is complete
        *   ½ way through control interface for lattice
        *   The hardest parts are complete
            *   Need tests from the old version
    *   Bill
        *   Wash-cli is complete, rpm / deb
            *   Want to test raspberry pi
        *   Wasccd getting a few errors for cross compile
        *   Next: Homebrew
        *   next^next^: windows
        *   Coral is arch64 build
        *   Need a mac
            *   Big sur / cortiana packaging
    *   Phil
        *   Multi-language support for waPC
        *   SDK Question
            *   Need tinygo, assembscript, remainder of rust for first party actor interffaces
            *   [https://github.com/wascc/actor-interfaces](https://github.com/wascc/actor-interfaces)
            *   If we build an actor on the existing rust api i twill be binary compatible with the new code gen work, developer experience will be different
            *   Instead of single monolithic sdk, you can pick and choose for example the http interface
            *   Kevin own’s rest of Rust ones
            *   Phil, tinygo and assemblyscript
        *   Combining github?
*   wasmCloud Discussion
    *   waPC / wasccd / krustlet bindings / other glue
*   Proposed [wasmCloud Updates](https://docs.google.com/spreadsheets/d/10qULIn3xX0ek3jMMNabUQNynysaPGAjJBSAyQy4T1TI/edit?usp=drive_web&ouid=101371928835254145623)

**<span style="text-decoration:underline;">Open PRs / Issue Review</span>**



*   [https://github.com/wascc/wasccd/issues](https://github.com/wascc/wasccd/issues)
*   [https://github.com/wascc/wasccd/pulls](https://github.com/wascc/wasccd/pulls)
*   Other components?

**<span style="text-decoration:underline;">waSCC Topic Backlog</span>**



*   Architectural Decision Record
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

**<span style="text-decoration:underline;">Shared To Do:</span>**

What / Who / When



*   Krustlet & Crit followup, Chris & Ralph,
*   Blogpost list for community folks, Ralph
*   wasmCloud rewrite