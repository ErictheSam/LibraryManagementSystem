# LibraryManagementSystem

## Introduction

This project is a library management system, the project of OOP class.

## Dependencies

* Ubuntu

* `mongo-cxx-driver`（[git](https://github.com/mongodb/mongo-cxx-driver)）

## Build

make under the root directory
## Architecture

There are five parts of this project, which are

* `Core`

* `Database`：Contect with database 

* `Server`：Code running on the server

* `Controller`：Code running on local gadget, contacting with  `Server`

* `Client`：Contacting with the client

This is a proxy pattern architecture, where `Server`uses the interfaces of `Database`,`Controller`uses the interfaces of `Server`, and `Client` uses the interfaces of `Controller`.

## Distribution of work

Yuzhong Wang: Core/Database/Server

Yibo Shen(me): Controller/Client(command version)

Chen Yu: Client(GUI version)
