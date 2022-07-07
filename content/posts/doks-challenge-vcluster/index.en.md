---
title: "DigitalOcean Kubernetes Challenge and vcluster Sharing"
date: 2022-02-11T23:36:39Z
tags: ["digitalocean", "k8s", "kubernetes", "vcluster", "CNCF"]
showToc: false
TocOpen: false
draft: false
hidemeta: false
comments: true
description: "Digital Ocean K8s Challenge Sharing"
canonicalURL: "https://blog.alankan.dev/posts/doks-challenge-vcluster"
disableHLJS: false
disableShare: false
hideSummary: false
searchHidden: false
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
cover:
    image: https://www.digitalocean.com/_next/static/media/logo.87a8f3b8.svg
    relative: false # when using page bundles set this to true
    hidden: false # only hide on current single page
# editPost:
#     URL: "https://github.com/alank976/blog/tree/main/content"
#     Text: "Suggest Changes" # edit text
#     appendFilePath: true # to append file path to Edit link
---

I joined [a k8s challenge event organized by DigitalOcean in December 2021](https://www.digitalocean.com/community/pages/kubernetes-challenge) that I couldn't quite recall how I came across its ads 😅Anyways, I picked one of the suggested topics:
> Deploy a virtual cluster solution
>
> Install vcluster to test upgrades (eg. 1.20 to 1.21 DOKS version) of your cluster. With a virtual cluster, you can create a new Kubernetes cluster inside your existing DOKS cluster, test the application in this new vcluster, and then upgrade your original cluster if everything works well with the new version.

I only have experience allocating namespaces per team/bounded context in my past and current day jobs. Although sharing cluster-wide resources like ingress controller is never a concern to us (yet, maybe?), it sounds interesting that I could see how things go virtualized on top of a well-known platform built for virtualization :joy: So I gave [vcluster](https://www.vcluster.com/) a shot.

I peeked at a bit other participants' work to gain some insight about how they illustrated their installation steps and learnings. Some used Infrastructure as Code tools like Terraform but I know nothing about it at all. That goes to the dummiest approach - words and GIFs 😅: https://github.com/alank976/doks-vcluster-challenge. Click into it if you are interested in what I had done :wink:

It was a great experience and I am grateful that DigitalOcean offered those topics and also CNCF and their cloud platform credits 💰. It is not much but I contributed nothing, learnt something, and took something away 😏.

What do you guys think about this spinner toy? Should I spend my credit on this little thing? I suspect the delivery fee might go beyond the credit I earned :joy:.
![](https://cdn.shopify.com/s/files/1/1300/8977/products/spinner_31a0980e-b9bf-40c5-8e5a-bd4f745bfb10_480x.jpg?v=1649701500)
https://store.cncf.io/products/the-kubernetes-metal-helm-fidget-spinner?_pos=6&_sid=7cc9dc1af&_ss=r
