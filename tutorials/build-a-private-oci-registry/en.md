---
SPDX-License-Identifier: MIT
path: "/tutorials/build-a-private-oci-registry"
slug: "tutorial-template"
date: "2024-10-11"
title: "Build a private OCI registry for your Docker images using Zod and Hetzner Object Storage"
short_description: "In this tutorial you will learn how easy it is to spin up a private OCI registry and how to scale it using Hetzner's Object Storage as backend"
tags: ["OCI", "Docker", "Object Storage"]
author: "Sven Pfennig"
author_link: "https://github.com/0xe282b0"
author_img: "https://avatars3.githubusercontent.com/u/....."
author_description: "" 
language: "en"
available_languages: ["en", "de"]
header_img: "header-x"
cta: "product"
---

## Introduction

Docker uses a registry to push and pull images, that registry is an Oci registry (link to Open Container Initiative). But in fact they can store arbitrary artifacts (oras) like helm charts(docs) or WebAssembly modules (link).
Popular free registry services are DockerHub, quay.io, and github container registry. But they are usually limited for private images (double-check). (Maybe refer to commercial offerings) 
In this tutorial you will learn how to set up your own private OCI registry, push and pull Docker images, helm charts and other artifacts and make it scalable using Hetzner Object Storage as backend. 

**Prerequisites**

- Docker
- Pulumi/Terraform if you want to automate your setup


For example:

* Hetzner Cloud [API token](https://docs.hetzner.com/cloud/api/getting-started/generating-api-token) in the [Cloud Console](https://console.hetzner.cloud/)
* [SSH key](https://community.hetzner.com/tutorials/howto-ssh-key)

**Example terminology**

Many tutorials will need to include example usernames, hostnames, domains, and IPs. To simplify this, all tutorials should use the same default examples, as outlined below.

* Username: `holu` (short for Hetzner OnLine User)
* Hostname: `<your_host>`
* Domain: `<example.com>`
* Subdomain: `<sub.example.com>`
* IP addresses (IPv4 and IPv6):
   * Server: `<10.0.0.1>` and `<2001:db8:1234::1>`
   * Gateway `<192.0.2.254>` and `<2001:db8:1234::ffff>`
   * Client private: `<198.51.100.1>` and `<2001:db8:9abc::1>`
   * Client public: `<203.0.113.1>` and `<2001:db8:5678::1>`

Do **not** use actual IPs in your tutorial.

## Step 1 - Summary of Step

Steps are the actual steps users will be taking to complete your tutorial.

Each step should build on the previous one, until the final step that finishes the tutorial.

It is important not to skip any steps, no matter how obvious or self-explanatory they may seem.

Feel free to include screenshots, to show exactly what the user should be seeing. Please put screenshots in a separate "images" folder.

The amount of steps will depend entirely on how long/complicated the tutorial is.

## Step 2 - Summary of Step

Quick introduction.

Start by...

![Screenshot Description](images/screenshot_description.png)

Then...

Finally...

### Step 2.1 - Summary of Step

You can create code examples in nearly every programming language.
Just state the language after the first three backticks in your Markdown file.

Here is a code example

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```

### Step 2.2 - Summary of Step

Another code example

```python
s = "Python syntax highlighting"
print s
```

## Step 3 - Summary of Step (Optional)

Instructions for a step that is not necessary to complete the tutorial, but can be helpful.

## Step N - Summary of Step

Yet more instructions.

## Conclusion

A short conclusion summarizing what the user has done, and maybe suggesting different courses of action they can now take.

##### License: MIT

<!--

Contributor's Certificate of Origin

By making a contribution to this project, I certify that:

(a) The contribution was created in whole or in part by me and I have
    the right to submit it under the license indicated in the file; or

(b) The contribution is based upon previous work that, to the best of my
    knowledge, is covered under an appropriate license and I have the
    right under that license to submit that work with modifications,
    whether created in whole or in part by me, under the same license
    (unless I am permitted to submit under a different license), as
    indicated in the file; or

(c) The contribution was provided directly to me by some other person
    who certified (a), (b) or (c) and I have not modified it.

(d) I understand and agree that this project and the contribution are
    public and that a record of the contribution (including all personal
    information I submit with it, including my sign-off) is maintained
    indefinitely and may be redistributed consistent with this project
    or the license(s) involved.

Signed-off-by: [submitter's name and email address here]

-->
