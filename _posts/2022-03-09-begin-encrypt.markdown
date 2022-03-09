---
layout: post
title:  "begin encrypt!"
date:   2022-03-09 11:58:00 -0800
categories: encryption cryptography nodejs mdn
---

# begin encrypt!

---

## `handshake` is born

[![white5moke/handshake](https://img.shields.io/badge/goto>-handshake-blue?style=for-the-badge "tooltip")](https://github.com/white5moke/handshake/)

so i decided to delve back into javascript after 5 years of bascially ignoring it. wow i was in for a rude awakening as far as relearning curves are concerned. here's [*handshake*](https://whit5moke.github.io/handshake/), a [nodejs](https://nodejs.org/) driven webapp for messing about with encryption for identity management. WIP be warned.

## web crypto api? do it.

after having hit a wall with nodejs' inability to provide a web-client based cryptography library. well, at least all of it, because all the important stuff like creating keys and warpping them, and such are only available on the system's side. so i stumbled upon, the [Web Crypto API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Crypto_API) provided by *MDN*. it's not as robust as node's, but has the necessary bits to get signing and encryption done. I especially like that most all key data is stored in `ArrayBuffers`. these are very useful for streamlining the key-to-identity pipeline. no one cares about the data, just as long as it works, so keep them as distilled as possible.

VALUE IS SOUL!