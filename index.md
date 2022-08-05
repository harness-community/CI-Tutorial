---
layout: page
title: Getting Started with Harness.io Continuous Integration
---

![A lovely image of our beloved Captain Canary](/assets/images/canary.png)
Hi!, I’m Captain Canary.
 I’ll be your friend and guide in this exercise. For your safety, please keep all your hands, feet and feathers inside the guide at all times. In this guide we’ll walk through building, testing and deploying our sample app. This app uses the MERN stack and is designed for your Kubernetes cluster. The code for the application is this repository: [harness-apps/MERN-Stack-Example](https://github.com/harness-apps/MERN-Stack-Example). Meanwhile, the DevOps/GitOps configuration is in the [harness-apps/MERN-Stack-Example-GitOps](https://github.com/harness-apps/MERN-Stack-Example-GitOps) repository.

I designed this guide for two groups. First, developers who are experienced with CI, but new to Harness. Secondly, for developers who are new to both CI and Harness. That said, This guide isn’t a one-size fits all situation. It’s focused on getting you up and running with Harness CI for a very specific application. Specifically, we will use our MERN stack getting started app. Keep that in mind, as you translate what we do to things your app does, or does not, need. I'll try not to assume prior knowledge. But we also don’t want to bore you to death with information and details you already know.
 
I've broken this guide down into topic based sections. Each section introduces the what and why of the actions you need to take. At that point, if you feel comfortable with the what and why, you’re free to take the red pill💊, login and make it so. If, on the other hand, you’re feeling a bit lost, that’s ok; it’s just my dashing good looks distracting you. Never fear, each section also has a more traditional follow-the-bouncing-ball ⚽ in depth section.

Before we take off🛫, there are a few things you need. Remember, this guide is specific to our MERN stack app. Your app may have different pre-flight steps.
## 🛫 Pre-flight checklist

- A Version Control System account 👩🏾‍💻. In this guide we’re going to use GitHub. Our example app’s source is on GitHub and you’ll need to fork those repos, so make sure you have a 🆓 GitHub account. Alternatively, if you’re comfortable following your inner-shoulder-angel’s guide to converting GitHub instructions you can use your own VCS. This, however, is an exercise for the reader. 
- A 🆓 Docker Hub account. Harness helps you publish container images virtually anywhere. For this guide we’ll use Docker Hub.
- Kubernetes cluster. You k8s cluster can run anywhere, so long as it has access to the internet. Later on you’ll create a ‘`demo`’ namespace. (yeah, naming things is hard 🙇‍♀️) Make sure that namespace is available. (Or you can JIT Translate in your head) 
  > Note, you need to be able to execute `kubectl` commands on your cluster, so make sure you’ve authenticated.
- MongoDB Atlas instance. Our MERN stack app uses Mongodb Atlas, as its datastore. You’ll need to [sign up 🆓 and get the connection URL from the Mongo Atlas interface.](https://www.mongodb.com/atlas/database) Helps to copy paste that to a notes file.

<a class="btn btn-primary" href="Forking/forkingTheRepos">👏 Ok, I've got those things, let's get started</a>