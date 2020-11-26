**<span style="text-decoration:underline;">waSCC Community Meeting - 2020-11-18</span>**

**<span style="text-decoration:underline;">Attendees</span>**
*   Kevin Hoffman
*   Liam Randall
*   Brooks Townsend
*   Phil Kedy
*   Chris Marshall
*   Ralph Squillace
*   Matt Fisher
*   Kevin Zhang


**<span style="text-decoration:underline;">Goal</span>**

Enable developers to build their functions and services in webassembly and run them everywhere.

**<span style="text-decoration:underline;">Introductions</span>**



*   Kevin Zhang
    *   Working on http://tearust.com

**<span style="text-decoration:underline;">Community News</span>**


*   [Meeting Recording](https://www.youtube.com/watch?v=sxT9VlIBCto&feature=youtu.be)
*   [Wasmtime Meeting Notes](https://docs.google.com/document/d/1ZtxZNWbTNIhDdIXt27NQdwuc6D5O288l5HZKc_wC0FQ/edit)
    *    wasi-nn merge, precedence setting
    *   Meta RFC-RFCs
    *   Release processes
        *   Lot wrapped up here; security releases; reporting, responding, etc
    *   Language bindings, pin versions to wasmtime version
        *   Neither Mozilla nor Fastly are using the rust crate
        *   Will be future target commit point; everything else will burn
*   Krustlet
    *   Continuing to evolve
*   Networking / wasi (Ralph)
    *   MS & Fastly (Pat) discussing experimental namespace for wasi networking
    *   BSD Sockets PR; complicated build process atm
    *   Want experiments and lessons learned
    *   Positive Community feedback around getting feedback
    *   To Do:
        *   Make explicit that this is experimental / more / less work
        *   Deliver it; needs more work
    *   Luke, Lynn & Till → 
        *   Publishing some technical blogposts and technical work
        *   Examples: wasi & cgi
        *   Maybe drop in a schedule of blog posts for experiments
        *   Maybe drive some community blogging

**<span style="text-decoration:underline;">waSCC Current</span>**



*   Kevin, .15 Core rewrite, Dec 7th
*   Bill, Packaging, Dec 7th
    *   New repository coming
    *   Target packages
*   Brooks, OCI (Dec 7)
    *   New OCI push functionality coming to [oci-distribution](https://github.com/deislabs/krustlet/pull/453)
*   Brooks, wash cli, (Dec 7)
    *   OCI push/pull functionality implemented under `wash reg`
*   waPC Code Generator, Phil Kedy (Dec 7?)
    *   From a waSCC standpoint you don’t even need to know it exists
    *   WIDL is pretty simple / easy to articulate your interface & go from there
    *   For first party providers, can use tiny crates for schema
    *   Ex: If building a http server, just use the http server crate
    *   For custom: you design schema in wild, and go from there
*   Krustlet, Matt Fisher
    *   Trying to finish out the rest of the kublet api
        *   Storage, networking interface, etc
        *   In a good position to build out demonstrations
        *   Focus on lower level infrastructure for now
        *   Thinking through how: do we tie into waSCC for example
        *   Additional provider (re krustlet slack)
            *   Running raw binaries from nodes
        *   Taylor working on storage, matt on crate so may be leveraged in crates
        *   Re waSCC; we could take k8s storage drives and see volume mounts
            *   Ex: container storage driver for azure / open stack etc/ wascc would get that for free
*   Dec 7 Script: WorkShop Walkthrough
    *   Already have feedback on this
    *   Ralph
        *   With the things like the CRI; banging against container native solutions (think CNAB & Porter)
        *   We should call out what it does provide which is network effect & ease of use
        *   Ex:
            *   Krustlet helps connect wasm to the container community
            *   But sketch out the boundaries
*   OCI Distribution
    *   Matt Fisher
        *   [https://blog.bacongobbler.com/post/2019-01-25-distributing-with-distribution/](https://blog.bacongobbler.com/post/2019-01-25-distributing-with-distribution/)
        *   
*   Open PRs
*   Open Issues

**<span style="text-decoration:underline;">waSCC Topic Backlog</span>**



*   Architectural Decision Log
*   Docs Rewrite
*   wasmCloud
*   Krustlet larger update
*   ADL (Architecture Decision Log)
    *   [https://wascc.github.io/adr/](https://wascc.github.io/adr/)
    *   ADL for register usage
*   Katakota Tutorials
*   Krustlet / wasm3 on small devices
    *   Constrained & JIT experience issues

**<span style="text-decoration:underline;">Shared To Do:</span>**

What / Who / When



*   Krustlet & Crit followup, Chris & Ralph,
*   Blogpost list for community folks, Ralph, 
