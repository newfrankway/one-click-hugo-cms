---
title: OpenVSCode Server
date: 2022-06-07T15:53:40.173Z
description: This project provides a version of VS Code that runs a server on a
  remote machine and allows access through a modern web browser. It's based on
  the very same architecture used by Gitpod or GitHub Codespaces at scale.
---
## Why?

VS Code has traditionally been a desktop IDE built with web technologies. A few years back, people started patching it in order to run it in a remote context and to make it accessible through web browsers. These efforts have been complex and error prone, because many changes had to be made across the large code base of VS Code.

Luckily, in 2019 the VS Code team started to refactor its architecture to support a browser-based working mode. While this architecture has been adopted by Gitpod and GitHub, the important bits have not been open-sourced, until now. As a result, many people in the community still use the old, hard to maintain and error-prone approach.

At Gitpod, we've been asked a lot about how we do it. So we thought we might as well share the minimal set of changes needed so people can rely on the latest version of VS Code, have a straightforward upgrade path and low maintenance effort.