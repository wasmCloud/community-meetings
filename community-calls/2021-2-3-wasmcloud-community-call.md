**<span style="text-decoration:underline;">wasmCloud Community Meeting - 2021-2-3</span>**

**<span style="text-decoration:underline;">Attendees</span>**


*   Liam Randall
*   Kevin Hoffman
*   Brooks Townsend
*   Chris Marshall
*   Bill Young
*   Matt Butcher
*   Matt Fischer
*   Taylor Thomas
*   Jared Overson
*   Radu Matei
*   Jordan Rash

##Goal

wasmCloud is a platform for writing portable business logic that can run anywhere from the edge to the cloud, that boasts a secure-by-default, boilerplate-free developer experience with rapid feedback loop.

**<span style="text-decoration:underline;">Introductions</span>**



*   

**<span style="text-decoration:underline;">Demo - </span>**



*   <span style="text-decoration:underline;">Kevin Hoffman, new docs: [https://wasmCloud.dev](https://wasmCloud.dev)</span>
*   Liam Randall, arch images: [https://jamboard.google.com/d/1ZBzr5y5OoG-4i-PfhdevbANEzmDgiabOtuEXGWeD1Xs/edit?usp=sharing](https://jamboard.google.com/d/1ZBzr5y5OoG-4i-PfhdevbANEzmDgiabOtuEXGWeD1Xs/edit?usp=sharing)
*   

**<span style="text-decoration:underline;">Community Activity</span>**



*   May 4, 2021 Cloud Native WASM CFP: [https://events.linuxfoundation.org/cloud-native-wasm-day/](https://events.linuxfoundation.org/cloud-native-wasm-day/)
*   [https://webassembly-summit.org/](https://webassembly-summit.org/)
*   April 22, 2021: https://webassembly-summit.org/
*   Kevin has an upcoming wasm talk in the UK
*   wasmTime bi-weekly meeting (Thursday’s 1:00
    *   [https://docs.google.com/document/d/1ZtxZNWbTNIhDdIXt27NQdwuc6D5O288l5HZKc_wC0FQ/edit#](https://docs.google.com/document/d/1ZtxZNWbTNIhDdIXt27NQdwuc6D5O288l5HZKc_wC0FQ/edit#)
*   Early Bird Kubecon & wasmDay registration through 2/14 only $10
    *   https://events.linuxfoundation.org/kubecon-cloudnativecon-europe/register/?utm_medium=email&_hsmi=109206644&_hsenc=p2ANqtz--i98lSj6l2kVU2BycNVfEJELqtwUp7kK0JBe2qqSp_2c7Y1dPc4xjRiL1GvTH9IU4a0F5snsR8_U91LEq9qhoiV9bLfA&utm_content=109206644&utm_source=hs_email
*   Open Call for additional items?

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


**<span style="text-decoration:underline;">wasmCloud Current</span>**



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
