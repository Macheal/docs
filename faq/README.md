---
title: FAQ
keywords: faq
tags: [faq]
sidebar: home_sidebar
permalink: /docs/faq.html
summary:
---

The FAQ should provide quick answers to the most common questions.

## What is Micro?

Micro is a framework for cloud native development. It addresses the key concerns for distributed systems and defines them as a set of 
services which act as the logical building blocks for microservices development.

## Where is the community?

There's a slack community with thousands of members. 

Invite yourself at [slack.m3o.com](https://slack.m3o.com/).

## Where do I start?

Start with the [getting started](getting-started) guide.

Browse through other directories for more info, join the slack to chat and look to [m3o.com](https://m3o.com) for a hosted offering.

## Who's using Micro?

See the [users](users) with a list of companies using Micro. 

Many more are also using it but not yet publicly listed. Feel free to add your company if you're using Micro.

## What do I use Micro for?

Use micro to build microservices. If you need to build Go based microservices in the Cloud then micro is the framework to start with.

## Where can I find examples?

Look at [github.com/micro/services](https://github.com/micro/services) for example services.

## What is local vs platform?

Micro supports Environments as a concept. An `env` is a micro server hosted somewhere either locally or elsewhere. It's defined 
as a name mapping to a host:port pointing to the micro proxy (gRPC proxy). We bake in two envs known as "local" and "platform". 

Local is your local server started with `micro server` and with the proxy on port :8081. Platform is an environment we're hosted 
in the cloud as a paid offering and ideally the place you'll run your code if you need hosting.

## Where can I run Micro?

Micro is runtime agnostic. You can run it anywhere you like. On bare metal, on AWS, Google Cloud. On your favourite container orchestrator like kubernetes.

As mentioned we run a platform [m3o.com](https://m3o.com) which offers Micro as a Service. If you need hosting head there.

## How performant is it?

Micro makes use of gRPC so it's about as performant as that. Micro also load balances between multiple instances of services 
and can offload to distributed systems infrastructure where scaling is necessary.

## Does Micro support gRPC?

Yes. In v2 and beyond micro makes use of gRPC by default.

## Micro vs Go-Kit

This question comes up a lot. What's the difference between micro and go-kit?

Go-kit describes itself as a standard library for microservices. Like Go, go-kit provides you with individual packages 
which can be used to construct your applications. Go-kit is great where you want complete control over how you define 
your services.

Go Micro is also a standard library for microservices so if you're looking to choose the best abstractions for the job 
check that out. Otherwise Micro is a framework for microservices, encapsulating all the requirements for backend 
and API development. Think of it like a platform.

## Where Can I Learn More?

Check out [Awesome Micro](https://github.com/micro/awesome-micro) for more resources.

{% include docs/links.html %}
