---
description: This page explains how to configure the Gryt Client
---

# 📃 Configuration

## Change Endpoint

Gryt Client comes with the ability for you to set your own endpoint. There are two ways to edit the endpoint of the _pre-built_ client: Through the settings menu in the application, located at the login-page, and by editing the configuration file located in its installation folder.

### In-App

You must be **logged out** in order to change which endpoint to connect to. \
Once you are at the login-page of the app, press the settings button _(the icon of a cog-wheel)_ in the bottom right of the login-frame. Replace the default endpoint with your servers IP-address/hostname and press **Apply**.

### With Configuration File

Make sure your application is **closed** before editing the settings-file.\
Locate the installation-folder of your client (usually located in %appdata%) and find the file called **settings.json**. Open the file and replace the endpoint with your servers IP-address/hostname. Save the file and start your application.

### Verifying Changes

Your client will now attempt to reach your new endpoint, and you should see a toast appear in the upper left corner with the message: _"🚀 Connected to socket"._&#x20;

_If you run into any trouble, check out the Troubleshooting section:_

{% content-ref url="../troubleshooting/handshake-issues.md" %}
[handshake-issues.md](../troubleshooting/handshake-issues.md)
{% endcontent-ref %}
