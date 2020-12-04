

**<span style="text-decoration:underline;">waSCC Community Meeting - 2020-12-2</span>**

**<span style="text-decoration:underline;">Attendees</span>**

**<span style="text-decoration:underline;">Goal</span>**

Enable developers to build their functions and services in webassembly and run them everywhere.

**<span style="text-decoration:underline;">Introductions</span>**



*   New Members

**<span style="text-decoration:underline;">Community News</span>**

- Mike Zupper ( @MikeZupper )

**<span style="text-decoration:underline;">waSCC Current</span>**



*   ToDo Followup
    *   Krustlet & Crit followup, Chris & Ralph (hold? Chris out)

Blogpost list for community folks, Ralph, 



*   Ralph has a list of potential blogposts; will be circulating ideas and topics to write about in a rough time frame
*   [https://hackmd.io/C9NKF1IAR7ith6Sukg2DxQ](https://hackmd.io/C9NKF1IAR7ith6Sukg2DxQ)

.15 Review



*   Kevin
    *   Rewrite is almost complete
    *   One cli is linked up
    *   Has a REPL inside it
        *   Fetch / start / stop / set
*   Brooks
    *   Demo of new WASH cli
    *   Wash reg pull wascc.asurecr.io/redis:v0.9.1
    *   Downloading / pushing built into wash
    *   TUI smart logger widget helped creating terminal UI
        *   Can select log level we want to see
    *   Supports :wq and other ways to exit
    *   Ralph: you need to pull the developer experience up higher
        *   Super extension to get this inside of vs code
        *   Kevin: requirement on the tooling → repl has to be scriptable; and all shell commands have to support crate or RPC via NATs
    *   RADU: do we need json output for all commands
        *   Kevin: existing cli turn from friendly into JSON
        *   
*   Packages
    *   Apt / yum for arm64 and amdx86
    *   BREW on the way 
*   Chris
    *   Working on TUI
    *   Adding stuff to wash up
    *   Working with bill
        *   Wasm3 did not like current build process; trying to enable 
*   wasmCloud Discussion
*   Proposed [wasmCloud Updates](https://docs.google.com/spreadsheets/d/10qULIn3xX0ek3jMMNabUQNynysaPGAjJBSAyQy4T1TI/edit?usp=drive_web&ouid=101371928835254145623) → Web Site Review
*   Krust PR
    *   Brooks PR in & Radu will test
    *   https://github.com/deislabs/krustlet/pull/453
*   waPC pull request
    *   Radu
    *   Everyone is doing calling
*   What about the wasmcloud
*   ADL (Architecture Decision Log)
    *   [https://wascc.github.io/adr/](https://wascc.github.io/adr/)
    *   ADL for register usage
*   Demo Script for the new wasmCloud Experience:
    *   [https://docs.google.com/document/d/11QWnLiep4B3F2KOr7kYBNumgYqFVdXf6Jur_7tLTM04/edit?usp=sharing](https://docs.google.com/document/d/11QWnLiep4B3F2KOr7kYBNumgYqFVdXf6Jur_7tLTM04/edit?usp=sharing)

**<span style="text-decoration:underline;">Open PRs / Issue Review</span>**



*   [https://github.com/wascc/wasccd/issues](https://github.com/wascc/wasccd/issues)
*   [https://github.com/wascc/wasccd/pulls](https://github.com/wascc/wasccd/pulls)
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

**<span style="text-decoration:underline;">Shared To Do:</span>**

What / Who / When



*   Krustlet & Crit followup, Chris & Ralph,
*   Blogpost list for community folks, Ralph followup
*   wasmCloud rewrite
*   Jarrod - turbulence & work
*   Brooks / Radu follow up on 
    *   https://github.com/deislabs/krustlet/pull/453

Feedback



*   Do a scheduled demonstration first
*   Brooks demo was awesome
*   Community of businesses interested in webassembly
    *   Scheduling some time 
*   Ivan → ensure wasmcloud is in the tube
    *   Template for wasmcloud in there
    *   Is this the richest thing?  Migrate here
*   Gartner
    *   Governor & o’grady on the 
    *   Microsoft establishing press relationships
    *   Kate list
