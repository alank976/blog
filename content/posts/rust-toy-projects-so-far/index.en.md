---
title: "replace me"
date: 2022-07-10T02:15:38Z
tags: ["rust", "wasm", "cloudflare-worker", "faunadb"]
# author: "Me"
showToc: false
TocOpen: false
draft: true
hidemeta: false
comments: true
description: "Desc Text here...."
canonicalURL: "https://blog.alankan.dev/posts/REPLACE_ME"
disableHLJS: true # to disable highlightjs
disableShare: false
hideSummary: false
searchHidden: false
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
# cover:
#     image: "<image path/url>" # image path/url
#     alt: "<alt text>" # alt text
#     caption: "<text>" # display caption under cover
#     relative: false # when using page bundles set this to true
#     hidden: true # only hide on current single page
editPost:
    URL: "https://github.com/alank976/blog/tree/main/content"
    Text: "Suggest Changes" # edit text
    appendFilePath: true # to append file path to Edit link
---

Today, I decided to re-pick up learning Rust and the primary focus will focus on WebAssembly after inspiring a few read recently. But before that, I think reorganizing a bit what I had done so far might sound a good idea to help me refresh what I had learnt. So, this blog would talk about the toy projects I made in 2020-2021 😅wow, almost 2 years since the first one. Didn't realize that until now! Let's talk about these 3 toys I played with 👀


## [todo-service](https://github.com/alank976/todo-service)

In this project, the primary goal is to act as a RESTful API to serve CRUD requests for TODO items. I didn't aim to deploy this thing to any cloud so it was targeted to runwith its required infrastructure in a docker-compose environment only. The infrastructures are namely, just Postgres and Flyway for table schema bootstrapping. See more in the [docker-compose.yaml](https://github.com/alank976/todo-service/blob/master/docker-compose.yaml).

Then, in rust realm, the main libraries/frameworks I had used:
- actix web: to host a HTTP server
- serde: serialize/deserialize JSON payloads (not surprising)
- sqlx: to talk to Postgres in a generic way instead of other Postgres-specific library

### 1st Challenge: inconsistent async runtime
During writing this blog, I can still recall those frustrations I felt when I firstly saw the "Bring your own async runtime" thing. The HTTP server framework Actix has its own async runtime, while the sqlx uses async-std. I stuck with the "get started" guide from official Actix website so actix-rt and kept sqlx plain vanilla without async-std. This is one of the biggest :question: I have with Rust's async ecosystem... (Now I found sqlx supports also `runtime-actix-native-tls` feature flag I guess)

### 2nd Challenge: Dependency injection?
Thanks to my previous OOP experiences, soon after I found I modeled this toy project exactly like Spring framework does, using handlers as controllers, repository for persistence-related codes. Managing multiple "beans" like these isn't an easy job, so a dependency injection library/framework is the answer usually. However, Rust is not really an OOP language, though it has similar "inheritance" concept but pretty different from its nature. 

I 

## commuter-service

## vocab-mate (private)