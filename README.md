# ❇️ Clark Ritchie

A Senior Staff Platform / Site Reliabilty Engineer with a diverse background of experiences.  Hands-on building and operating scalable SaaS cloud-native systems for over 15 years as both an IC and leader.

I am passionate about building and operating **world-class applications** that **delight its end users**.

Connect with me on:
- [LinkedIn](https://www.linkedin.com/in/clarkritchie)
- [GitHub](https://www.github.com/clarkritchie)

## 💬 TL;DR

- Core skills:  Linux, Kubernetes, Python, Go (Golang), infrastructure as code (Pulumi, Crossplane, Terraform), CI/CD, cloud (GCP, AWS), observability (Datadog), and loads of experience with tools like GitHub Actions
- I am a developer, but also very close to infrastructure
- I approach software development with an SRE's mindset -- scalability, fault-tolerance, optimizing spend, monitoring and alerting -- these things, and more, are always part of my thinking
- Sometimes good is better than perfect; I like to ship early and ship often
- Let's go!

## 📌 Career TL;DR

- BS in Computer Science, Univ. of Puget Sound ('96)
- Early career — Intel factory automation, Hewlett-Packard, a startup (’96-’11)
- MS in Computer Science, Oregon State Univ. ('01)
- Experience at 4 startups
- 12 years writing software for fixed wireless networks in US low-income and throughout East Africa, Haiti, The Philippines
- Co-founded an [ISP in Kenya](https://pitchbook.com/profiles/company/113840-47) (’13-’18)
- 5 Years as Platform Engineer at [Specialized Bicycle Components](https://www.specialized.com/us/en) (’18-’23)
- Principal Engineer at Blueboard, a failed HR SaaS startup (’23-’24)
- Senior Staff SRE Software Engineer at [Dexcom](https://www.dexcom.com) ('24-present)

## Current Stack

These days I am using Kubernetes (GKE), Helm charts, GitHub Actions, Python, Go, GCP (Cloud Run, Secret Manager, Cloud SQL, Spanner) and Datadog.

For infrastructure as code it is mostly Pulumi and Crossplane.  A lot of my recent work is observability as code -- managing Datadog monitors, synthetics and service level objectives across dozens of environments in three global regions, plus the Python service that runs the synthetics themselves.

I also spend a fair amount of time on AI-assisted engineering workflows -- reusable skill definitions, repo-level agent instructions, and permission guardrails that keep destructive cloud and state operations under human review.

## 🗒️ Random Things on my GitHub

**Dislcaimer:** This is all very, very old!!!

A lot of this is elementary stuff -- sometimes I use these just to prove out a basic concept or maybe to provide myself a template for future use.  Some of the Terraform is more sophisticated.

- [VS Code Dev Containers](https://github.com/clarkritchie/etc/blob/main/vscode-dev-containers/README.md)

### Go Things

- [Basic Go Things](https://github.com/clarkritchie/basic-go-things)
  - [gRPC](https://github.com/clarkritchie/basic-go-things/tree/main/grpc) -- gRPC example of a "Hello World" server in Go, with clients in Go and Python
- Produce [camelCased JSON from a Go Struct](https://gist.github.com/clarkritchie/e98791cfb06f6fcd22e40ddb2516376c) -- I was asked in an interview how to do this... I've always referred to this technique as "JSON Hints", but maybe that's incorrect?  I think that `json.Marshal` was all they were looking for.

### Terraform Things

  - [GitHub](https://github.com/clarkritchie/terraform-things/tree/main/github-clarkritchie) for doing things with GitHub repos
  - [s3-static-hosting](https://github.com/clarkritchie/terraform-things/tree/main/s3-static-hosting) Very simple web hosting on S3, no https
  - [s3-remote-state](https://github.com/clarkritchie/terraform-things/tree/main/s3-remote-state) Terraform to create the Terraform backend state on AWS, so meta
  - The [Docker Swarm section](https://github.com/clarkritchie/terraform-things/tree/main/docker-swarm) is a series of bespoke Terraform projects I made to create a VPC, subnets, EC2s, ELBs, bootstrap a Docker Swarm cluster, stand up Postgres and MySQL (Serverless) and Elasticache (Redis) instances, as well as SNS for alarms, and more
    - [aws-alarm-infrastructure](https://github.com/clarkritchie/terraform-things/tree/main/docker-swarm/aws-alarm-infrastructure)
    - [aws-docker-swarm](https://github.com/clarkritchie/terraform-things/tree/main/docker-swarm/aws-docker-swarm) -- This is the base layer, the others mostly use `outputs` from this
    - [aws-elasticache-redis](https://github.com/clarkritchie/terraform-things/tree/main/docker-swarm/aws-elasticache-redis)
    - [aws-mysql-rds](https://github.com/clarkritchie/terraform-things/tree/main/docker-swarm/aws-mysql-rds)
    - [aws-postgres-rds](https://github.com/clarkritchie/terraform-things/tree/main/docker-swarm/aws-postgres-rds)
  - [AWS Guard Duty](https://github.com/clarkritchie/terraform-things/tree/main/aws-guardduty) A truly minimalistic setup of Guard Duty

### Python Things

- [Basic Python Things](https://github.com/clarkritchie/basic-python-things)
- [Go shared lib](https://github.com/clarkritchie/basic-python-things/tree/main/go-shared-lib) -- The _Sieve of Sundaram_ in Python (native) versus it in Python, but with the heavy lifting done in Go (code compiled to a `.so` file)
- Quick and dirty Python script to [delete old branches](https://gist.github.com/clarkritchie/6be7d3d8fec96901002b01df2eaafb6e) -- this is more or less the the same thing in a [shell script](https://gist.github.com/clarkritchie/071a3cbced4f5286d751bce0099fed61)

### Docker Things

- [Kubernetes Things](https://github.com/clarkritchie/k8s-things) -- Hello world stuff from when I was just getting started with Kubernetes and Helm charts
- Simple [example](https://github.com/clarkritchie/pizza-store-app) of how you might use Docker Compose to run a small Fast API server that can reach a Maria DB database
- Shell script to [tag a container with a semvar+sha](https://gist.github.com/clarkritchie/600297e23a05a629664bfbff20d03b51)

### GitHub Actions Things

- Full example of the [GHA 'context' object](https://gist.github.com/clarkritchie/b84937c0c83bcf1de9f25ca63bcaf77a)
- Shell script to [delete all workflow runs](https://gist.github.com/clarkritchie/a3f193e93155d320e1a3c001cc4e43b5)
- Read Secure Notes from 1Password and push to GitHub Secrets (see above) [but in a GHA](https://gist.github.com/clarkritchie/843c54c66af0833d05a88ab6fd84a544) -- this is the way
- If you must do a [nested ternary](https://gist.github.com/clarkritchie/d3c35a9feeec5ed62ddbb38172ee62c2) in GHA
- Trick GHA into [revealing a secret](https://gist.github.com/clarkritchie/def05211e6dd0ec6a8e1edd48f0f822b) -- yes, this is possible!
- This is cool -- [use Python in a GHA step](https://gist.github.com/clarkritchie/a347d3fe9c72f47d9ece95f4dda38536)
- Trigger a GHA with a `workflow_dispatch` outside of the `main` branch [like this](https://github.com/clarkritchie/etc/blob/main/.github/workflows/run-outside-main.yaml)
- I made this Python script to [read Secure Notes from 1Password and push to GitHub Secrets](https://github.com/clarkritchie/1pw-github-secrets) -- this is very bespoke but is how I once used 1Password Notes as the "source of truth" for env vars which were stored as GitHub secrets (environment, repository or organization) -- this code was originally forked from someone else's project but heavily modified for my needs
- Example of how you might [lint in a GHA](https://gist.github.com/clarkritchie/2f935597b9398a34380e8c9a90005b6f) -- this example is for Terraform, but could be used to lint Python code with Ruff, etc.

### Random Things

- A few things that I made to make copying a Postgres db from [Heroku to RDS](https://github.com/clarkritchie/heroku-to-rds) a little easier
- [List, Copy, Delete S3 Bucket](https://gist.github.com/clarkritchie/fdce6b1a365ce176040bc8e7fca3a0c7)
- Cloudflare [maintenance page worker](https://gist.github.com/clarkritchie/31aa63566ac388332cb2a6275a40396d)
- [tickr-rpi-ws281x](https://github.com/clarkritchie/kickr-rpi-ws281x) -- This was a small side project to control a programmable LED light strip using heart rate data from a Wahoo TICKR heart rate monitor -- I never finished this... the Bluetooth to the TICKR part works, IIRC
- [Manage Cloudflare records](https://gist.github.com/clarkritchie/f518f5f7a8fb889f9fa9f87e7574cbe4)
- [Nexus 7 Deployment Script](https://github.com/clarkritchie/nexus7) -- Something I did over 10 years ago to speed up deploying a bunch of Google tablets
- Sort a [1Password Note](https://gist.github.com/clarkritchie/1e223f3cd3657cd00722be52f4249c1a) from the command line, uses the 1Password CLI
- [trails.losritchi.es](https://github.com/clarkritchie/trails.losritchi.es) is a tiny SPA (React) I made to help me name my mountain bike rides for Strava, it lives [here](http://trails.losritchi.es/)

Additional other random notes and code snippets that I did not explicitly link to are [here](https://gist.github.com/clarkritchie)