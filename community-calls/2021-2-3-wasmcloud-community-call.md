**<span style="text-decoration:underline;">wasmCloud Community Meeting - 2021-2-3</span>**

**<span style="text-decoration:underline;">Attendees</span>**



*   

**<span style="text-decoration:underline;">Goal</span>**

Enable developers to build their functions and services in WebAssembly and run them everywhere.

**<span style="text-decoration:underline;">Introductions</span>**



*   

**<span style="text-decoration:underline;">Demo - </span>**



*   

**<span style="text-decoration:underline;">Community Activity</span>**



*   CFP: [https://events.linuxfoundation.org/cloud-native-wasm-day/](https://events.linuxfoundation.org/cloud-native-wasm-day/)
*   [https://webassembly-summit.org/](https://webassembly-summit.org/)
*   wasmTime (Thursday’s 1:00
*   Run time working group

**<span style="text-decoration:underline;">wasmCloud Deployment Options</span>**



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
