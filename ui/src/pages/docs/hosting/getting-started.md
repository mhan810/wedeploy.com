---
title: "Getting Started"
description: "Serve static files easily using WeDeploy™ Hosting."
headerTitle: "Hosting"
layout: "guide"
weight: 1
---

# Hosting

###### {$page.description}

<div class="guide-btn-cta">
  <a class="btn btn-accent btn-sm" href="http://boilerplate-hosting.wedeploy.io" target="_blank">
    <span class="icon-16-external"></span>See Live Demo
  </a>
</div>

<div class="guide-aux-cta">
  or read the <a href="https://github.com/wedeploy/boilerplate-hosting" target="_blank">source code</a>.
</div>

<article id="1">

## Install dependencies

This section assumes that you already have the **WeDeploy CLI** installed and **Docker** running. Make sure to [visit the installation guide](/docs/intro/using-the-command-line.html) if you need help setting that up.

</article>

<article id="2">

## Running locally

WeDeploy™ provides a way to run your project locally using a sandbox system.

1. Start local infrastructure:

```xml
we run
```

2. Clone this repository:

```xml
git clone https://github.com/wedeploy/boilerplate-hosting.git
cd boilerplate-hosting
```

3. Link this container with the local infrastructure:

```xml
we link
```

4. Now your container is ready to be used:

```xml
http://hosting.<projectID>.wedeploy.me
```

Inside this project folder, you can find a `container.json` with the container ID used in this case: `hosting`.

</article>

<article id="3">

## Deploying to the cloud

1. [Fork this repository](https://github.com/wedeploy/boilerplate-hosting/fork).

2. Go to the [Dashboard](http://dashboard.wedeploy.com) and create a project.

3. In the sidebar, click on *Deployment*.

4. Using your local machine, clone your Github fork:

```xml
git clone https://github.com/<username>/boilerplate-hosting
```

5. Get into the folder: `cd boilerplate-hosting`.

6. Using the content on *Deployment* page. Add the WeDeploy remote url:

```xml
git remote add wedeploy http://git.wedeploy.com/<projectID>.git
```

7. Push your data to wedeploy git server: `git push wedeploy master`.

8. Once you see it in the Dashboard, your container will be ready to be used.

```xml
http://hosting.<projectID>.wedeploy.io
```

</article>

<article id="4">

## Error pages

Files put into the special directory `/_error` are mapped as the error files to be served in case of an error. They must take the form of `<error code>.html`.

</article>

## What's next?

* Now you can start adding new static files and grow your application.
