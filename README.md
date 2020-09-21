# MERN Suggestions App

You've probably heard of full-stack development before.

Briefly, it's a ubiquitous term that encapsulates both backend and frontend development (server-side and client-side, respectively) into one neat developer.

There are some arguments that go into the effectiveness of such a model, but that's neither here nor there.

As a precursor to writing blockchains, smart contracts, and decentralized apps, we need to go back to basics.

## Environment Setup

Before we begin, we need to make sure that everything necessary is installed.

1. Download [Git](https://git-scm.com/downloads), if you haven't already. We'll use this for version control and pushing files to GitHub. After downloading, check that everything works by running `git --version` in the terminal; there should be no errors.
2. Download [Node.js](https://nodejs.org/en/download/). We'll use this for our applications' backend. Check that everything works by running `node -v` and `npm -v` in the terminal---they should only output the version number.
3. Download [MongoDB](https://www.mongodb.com/download-center/community). We'll use this as the framework for our database. 
4. Download an IDE that you're familiar with. We recommend using [Visual Studio Code](https://code.visualstudio.com/) if you're unsure about what you want.

## Project Overview

This project is more of a tutorial than anything; while you may not make anything that will impress anybody yet, this project will give an overview on how to code in JavaScript, targeting both the backend and the frontend. More specifically, we'll be creating a suggestions web app using the MERN stack&mdash;MongoDB, Express, React, and Node&mdash;where a user can create a suggestion with a couple fields and view all currently-posted suggestions. In other words, we'll be creating and reading data.

For a more in-depth idea of how to complete the project, read the [wiki](https://github.com/blockchainpsu/mern-suggestions/wiki) and read through the details. It'll guide you through the steps, including some of the underlying theory of how information is moving and actual code snippets.

Solutions are included in the appropriately-named `solutions` folder, while the actual project itself is in the `suggestion-app` folder.

If you have any troubles working through the project, feel free to reach out to anybody on the Blockchain@PSU team.

## Links

- [Email](mailto:blockchain.psu@gmail.com)
- [Slack](https://tinyurl.com/blockchainpsu-slack-fa20)
- [Website](https://blockchainpsu.com)
- [JS Cheet Sheat](https://htmlcheatsheet.com/js/)

## Brief Background

#### Requests and API Calls

**Requests** allow the client to communicate with the server, often asking for specific bits of data from a database to be displayed on the client.

There are two different types of requests that return data: **GET** and **POST**.

**GET** methods request for data from the server by appending the arguments to the URL. When you search something on Amazon, you'll see it return a URL with `?k=searchterm` appended to the end of it. That's the GET request asking for data from the server.

**POST** methods are more complicated; instead of appending their arguments to the URL, the arguments are appended to the HTTP request. A sample POST request could look something like the following:

```
POST / HTTP/2.0
Host: foo.com
Content-Type: application/x-www-form-urlencoded
Content-Length: 13

say=Hi&to=Mom
```

#### API Calls

An **API** (application programming interface) exists to move data from your server to your client. When we say that you're make an API call, it means the web app sends a request to the API (server) for data.

So if you think about it, in a full-stack application, part of my backend will inevitably be devoted to creating an API.

#### Web Sequence Diagram

Before we begin creating a web app, we need to understand the fundamentals and, more importantly, the flow of information through your app.

Full-stack development involves the creation and maintainence of several layers behind your app. In most cases, there will be three layers: the client (frontend), server (backend), and database. Web sequence diagrams are very helpful when trying to understand how information moves from one layer to the next.

![web sequence diagram](https://raw.githubusercontent.com/blockchainpsu/blockchain-essentials-spring2020/mern/part1/websequencediagram.png)

####  Additional Information

Some of this information was shamelessly taken from Mozilla's tutorial [here](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data), if you'd like to read more.
