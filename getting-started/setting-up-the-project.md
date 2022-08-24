---
description: This page describes how to setup the Gryt Client for development
---

# ✨ Setting up the project

{% hint style="warning" %}
## Requirements

_You must have these installed on your system in order to setup, develop and build the project_

* [NodeJs](https://nodejs.org/en/)
{% endhint %}

## Cloning the repository

Begin by opening a terminal and executing the following command to clone the repository:

```git
git clone https://github.com/Gryta-Krutt/client.git
```

Now we can step into our cloned repository using the cd-command:

```bash
cd client
```

Next up, let's install all dependencies with:

```bash
npm i
```

## Starting the client

You can start the client by executing the following command; inside the project directory (_client_-folder):

```bash
npm start
```

## Configuring the client

Create a new file inside the _client_-folder and give it a name of **.env** exactly. Inside of this file, place these variables:

```bash
# Endpoint Properties
SOCKET_ADDRESS = localhost:2700

# Registration Properties
PASSWORD_MIN_LENGTH = 5
```

`SOCKET_ADDRESS` defines the default endpoint for your client. This endpoint is used if no other endpoint is set in the settings.json-file.

`PASSWORD_MIN_LENGTH` defines the minimum length allowed when registering a new user. This applies to both the login- and register-page.
