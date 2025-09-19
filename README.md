# Lets Go — Portfolio Overview

I co-founded and built the product for a two-person startup for ~3 years. I owned the software side end-to-end while my partner ran the business (operations, sales, customer development). This page highlights the architecture and links to the key repositories.

<p align="center">
  <img src="LetsGoAppOverview.drawio.svg" alt="Lets Go Architecture" width="900">
</p>

## Highlights (skim me)
- **My role:** system design, backend (C++), Android (Kotlin), matching engine, integrations, server administration, deployment docs.
- **Architecture:** stateless C++ **Application Server** (gRPC/Protobuf) with **MongoDB**.
- **Matching:** Mongo **aggregation pipeline** + **C++ converter** for embedded execution and speed.
- **Clients:** Android app for end users and a **Desktop Admin Interface (Qt)** for moderation/ops and event tools.
- **Integrations:** SMS + Email providers for notifications and verification as well as account flows.

## Highlighted Repositories
- **Server (C++)** — stateless hub, gRPC/Protobuf, MongoDB  
  👉 [`Lets_Go_Server`](https://github.com/lets-go-app-pub/Lets_Go_Server)

- **Android Client (Kotlin)** — auth, profiles, activities, chat *(SDK versions may be dated)*  
  👉 [`Lets_Go_Android_Client`](https://github.com/lets-go-app-pub/Lets_Go_Android_Client)

- **Desktop Admin (Qt)** — admin/ops console for moderation, events, stats, and controls  
  👉 [`Lets_Go_Interface`](https://github.com/lets-go-app-pub/Lets_Go_Interface)

- **Matching (Algo & Converter)** — Mongo aggregation (JS) + C++ converter to embed pipelines  
  👉 [`Lets_Go_Algorithm_And_Conversion`](https://github.com/lets-go-app-pub/Lets_Go_Algorithm_And_Conversion)

- **Protobuf Files** — protobuf files used to communicate between server and clients  
  👉 [`Lets_Go_Protobuf`](https://github.com/lets-go-app-pub/Lets_Go_Protobuf)

- **Docs & Deployment Notes** — release checklists, SSL testing, Mongo RS commands  
  👉 [`Lets_Go_Docs`](https://github.com/lets-go-app-pub/Lets_Go_Docs)

## What I did
- **Architecture & backend:** designed the system, authored most server code, defined gRPC/Proto contracts.
- **Data & matching:** wrote aggregation pipelines and the C++ converter to run them efficiently server-side.
- **Android:** implemented core UI/flows (auth, profiles, activities, chat).
- **Admin interface:** contributed features and workflows used for moderation and operations.
- **Server administration:** provisioned Linux hosts, configured system services, SSL/TLS, backups, and monitoring; operated a MongoDB **replica set** across separate nodes.
- **Integrations:** wired SMS and Email providers for notifications and account flows.

## Status & scope
- Active development ~3 years.
- The company is **sunset**, and this code is provided for anyone that it may have value to as well as for **portfolio** purposes.
- Tooling notes: Android project targets older SDKs; the **Desktop Admin uses Qt** (modern builds may require current Qt tooling/licensing).

## Tech at a glance
`C++ · gRPC · Protobuf · MongoDB (Replica Set) · Android (Kotlin) · Qt · Aggregation Pipelines · SSL/TLS · Gradle/CMake · Linux Server Ops · Wordpress`

