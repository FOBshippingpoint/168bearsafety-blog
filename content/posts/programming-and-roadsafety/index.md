---
weight: 1
title: "從程式語言來看交通安全設計"
date: 2023-01-20T16:18:39+0000
lastmod: 2023-01-20T16:18:39+0000
draft: false
author: "熊安全"
# authorLink: ""
description: ""
resources:
  - name: "featured-image"
    src: "feat.webp"
  - name: "featured-image-preview"
    src: "feat_preview.webp"

tags: ["交通安全設計"]
categories: ["其他"]

lightgallery: true

toc:
  auto: false
---

memory safety（記憶體安全）一直是很重要的問題，在 C、C++這類可以直接操控記憶體的語言就存在者 memory safety problems，讀到錯誤的資料、覆蓋到別人的資料...等等，Android 的九成錯誤都是因為記憶體操作不當造成的[^1]。

雖然經驗豐富的工程師可能可以避免設計出不安全的程式，但其實還有另一個選項：使用 memory safety 的程式語言。像是 JavaScript、Rust、Python 之類的，從「設計」上就迴避掉了犯錯的可能，如果對 C、C++還是有需求，也可以用其他輔助手段減輕問題。

類似的概念可以套用到交通安全上，我們的基礎設施、法制如同不安全的 C、C++一樣，縱使經驗豐富的用路人也可能會在不安全的環境下犯錯，軟體犯錯不會出人命，但在道路上會！從最安全的車輛行人時相分離來講，就像 memory safety language 一樣，根本上防止危險的發生，若一時無法遷徙到安全的體制上，也可以用標線型人行道來暫時緩解問題，但是要記住，不安全的設計不管人們再怎麼小心總有一天還是會出事。


[^1]: https://security.googleblog.com/2019/05/queue-hardening-enhancements.html
