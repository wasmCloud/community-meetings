**<span style="text-decoration:underline;">wasmCloud Community Meeting - 2020-12-16</span>**

**<span style="text-decoration:underline;">Attendees</span>**

**<span style="text-decoration:underline;">Goal</span>**

Enable developers to build their functions and services in webassembly and run them everywhere.

**<span style="text-decoration:underline;">Introductions</span>**



*   Andrew Brown, Intel, Wasi-NN
*   Mingqui Sun, Intel, Wasi-NN

**<span style="text-decoration:underline;">Demo</span>**



*   Wasm Berkeley Sockets API, Radu Matei
    *   Experimental branch supporting sockets
    *   [https://radu-matei.com/blog/towards-sockets-networking-wasi/](https://radu-matei.com/blog/towards-sockets-networking-wasi/)
*   Great Back Ground:
    *   [https://github.com/WebAssembly/WASI/pull/312](https://github.com/WebAssembly/WASI/pull/312)
*   Awesome post: 
    *   [https://engineering.linecorp.com/en/blog/adding-experimental-webassembly-support-to-decaton-part-1/](https://engineering.linecorp.com/en/blog/adding-experimental-webassembly-support-to-decaton-part-1/)
    *   [https://engineering.linecorp.com/en/blog/adding-experimental-webassembly-support-to-decaton-part-2/](https://engineering.linecorp.com/en/blog/adding-experimental-webassembly-support-to-decaton-part-2/)
*   Very simple implementation
    *   Does not look at capabilities
    *   Simply returns handle to file
    *   Easiest to get started with Assemlby script
*   Does require special build of wasmtime
    *   And a patched standard library from the rust compiler
*   

<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image1.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image1.png "image_tooltip")

    *   On the roadmap
        *   Capabilities (protections) for
            *   Requesting a socket
            *   IP range, port range
        *   The whole approach to this works for clients - but with out multi-threading not really efficient for server approaches
            *   (if only there were a multi-threaded application runtime that enables parallel single threaded execution)
        *    

**<span style="text-decoration:underline;">Community News</span>**



*   wasmTime community meeting is Thursday 12/24 at 1:00
    *   [Meeting Agenda](https://docs.google.com/document/d/1ZtxZNWbTNIhDdIXt27NQdwuc6D5O288l5HZKc_wC0FQ/edit#)
    *   Maybe cancelled - xmas eve
*   Deis Labs
*   Wasi-nn blog post
    *   [https://bytecodealliance.org/articles/using-wasi-nn-in-wasmtime](https://bytecodealliance.org/articles/using-wasi-nn-in-wasmtime)
    *   Ref: [https://radu-matei.com/blog/tensorflow-inferencing-wasi/](https://radu-matei.com/blog/tensorflow-inferencing-wasi/)
*   

**<span style="text-decoration:underline;">wasmCloud Current</span>**



*   ToDo Followup
    *   Krustlet & Crit followup, Chris & Ralph (hold? Chris out)
*   Brooks / Radu follow up on 
    *   [https://github.com/deislabs/krustlet/pull/453](https://github.com/deislabs/krustlet/pull/453)
*   Jarrod - turbulence & work
    *   Outline tickets

Blogpost list for community folks, Ralph, 



*   Ralph has a list of potential blogposts; will be circulating ideas and topics to write about in a rough time frame
*   List of potential blogposts:
    *   [https://hackmd.io/@y7qXqYh2SdqS3oy5XujVDA/B1Q1qISjw](https://hackmd.io/@y7qXqYh2SdqS3oy5XujVDA/B1Q1qISjw)

.15 open tickets



*   Remaining To do on .15
    *   [Actor-interfaces](https://github.com/wasmCloud/actor-interfaces/issues)
        *   4 Rust
        *   7 Go
        *   7 Assembly Script
    *   Wash up / REPL
    *   Packaging
        *   Home Brew
    *   Automation for builds on wasmCloud repo
        *   Don’t have automated testing on repo
        *   Need the action step
    *   wasmCloud.com website
    *   Azure Registry
        *   wasmCloud
*   Chris
*   Brooks
*   Bill
*   Phil
*   Demo Script Updates for the new wasmCloud Experience:
    *   [https://docs.google.com/document/d/11QWnLiep4B3F2KOr7kYBNumgYqFVdXf6Jur_7tLTM04/edit?usp=sharing](https://docs.google.com/document/d/11QWnLiep4B3F2KOr7kYBNumgYqFVdXf6Jur_7tLTM04/edit?usp=sharing)
*   Bindle release
    *   [https://github.com/deislabs/bindle/](https://github.com/deislabs/bindle/)
    *   

**<span style="text-decoration:underline;">Open PRs / Issue Review</span>**



*   [https://github.com/wasmCloud/wasmCloud/issues](https://github.com/wasmCloud/wasmCloud/issues)
*   [https://github.com/wasmCloud/wasmCloud/pulls](https://github.com/wasmCloud/wasmCloud/pulls)
*   ADL (Architecture Decision Log)
    *   [https://wasmcloud.github.io/adr/](https://wasmcloud.github.io/adr/)
*   

**<span style="text-decoration:underline;">waSCC Topic Backlog</span>**



*   Demo: wasi-nn Demo, Andrew Brown
*   Demo: WIDL, Phil Kedy
*   Demo: waPC, Phil Kedy
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



*   
