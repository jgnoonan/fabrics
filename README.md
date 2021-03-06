# Introduction

In this repository you will find a collection of predefined scripts to help you spin up fabric networks (locally or on the cloud) for educational purposes. The scripts have been intentionally kept as minimal as possible to ensure that it is easy to be understood by user and maintainable.

* [tiny](./tiny) - Scripts to create a network with 1 x orderer, 1 x org ( 1 x peer with couchDB)  and 1 x cli. No TLS.
* [tinyca](./tinyca) - Scripts to create a network with 1 x CA, 1 x orderer, 1 x org ( 1 x peer with couchDB) and 1 x cli, TLS enabled.
* [medium](./medium) - Scripts to create a network with 1 x orderer, 2 x orgs ( 1 x peer with couchDB per org) and 1 x cli. TLS not enabled.
* [e2e](./e2e) - Temporary copy of hyperledger fabric e2e example. The plan is to replaced this with a version capable of spanning multiple nodes (e.g. macs, VMs, etc) to mimic multiple organisations across physical nodes.

This list is not exhaustive and more will be added.

<hr>

<b> Warning </b>

This repo is subject to changes without warning. Clone or fork this repo to ensure that you have a copy. 

Modify the script to meet your needs as there is no intention extend the scripts to fit every possible use cases.

<hr>

# How to use these scripts



To used these scripts to your best advantage, it is recommended that you organise all your projects (Go and non-Go ones) around [Go workspace](https://golang.org/doc/code.html#Organization). All you need to do is to run the command `go get github.com/hlf-go/fabric` to download it to the your Go workspace:

```
$GOPATH/src/
    github.com/hlf-go/
        fabric/
```

If you need to reference the scripts from anywhere in the Go workspace, just reference it via `$GOPATH`. Likewise, from with the scripts you can also reference other resources in your Go workspace via `$GOPATH`.


# Disclaimers

The scripts provided here are intended to help you spin up fabric networks to support your local development and/or help you gain insights to what is involved in establishing a fabric network. There is no guarantee that these scripts are free from defects. 

These scripts are also NOT intended for used in any mission critical, corporate or regulated projects. Should you choose to use them for these types of projects, you do so at your own risk.

Unless otherwise specified, the scripts in this repository are distributed under Apache 2 license and are provided on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.