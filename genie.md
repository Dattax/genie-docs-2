# Hosting a Genie Application

## Getting Started with Genie Builder on JuliaHub

```@raw html
<iframe
    width="560"
    height="315"
    src="https://www.youtube-nocookie.com/embed/7qZwhxnzXPI"
    title="YouTube video player"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen
    style="width: 100%; aspect-ratio: 560/315"
></iframe>
```

## Introduction

On this page, we will demonstrate how to deploy a dashboard using Genie Builder for data-centric web applications.

## Getting Started with Genie Builder

1. First, Login to JuliaHub.com
2. Navigate to the Projects area (on the left-side panel)

<img width="1426" alt="s0" src="https://github.com/Dattax/genie-docs-2/assets/1408846/ca4e8c47-544c-4e0f-aa5c-995af7045525">

## Create a New Project:

<p>1. Click on "Create Project”</p>
<p>
<img width="1346" alt="s1" src="https://github.com/Dattax/genie-docs-2/assets/1408846/f3385821-5855-4b22-b33a-d646d0233417">
</p>
<p>2. Select Genie from the template choices</p>
<p>
<img width="1421" alt="s2" src="https://github.com/Dattax/genie-docs-2/assets/1408846/c27a87bf-6959-450d-b544-80758916e8ec">
</p>
<p>3. Give your project a name and (optional) description.  Select Editing Mode (Exclusive if working by yourself) or Collab Mode (if you want to have others work off branches on your project)</p>
<p>
<img width="1393" alt="s3" src="https://github.com/Dattax/genie-docs-2/assets/1408846/610f6292-796e-4327-bb9f-c5970636ce37">
</p>
<p>4. Add any Collaborators if needed</p>
<p>
<img width="1378" alt="s4" src="https://github.com/Dattax/genie-docs-2/assets/1408846/f496a8a1-582e-44ea-b844-c49578a4bf86">
</br>
<p>5. Once your project is created, hit the Launch button.<p>
<p>
<img width="1328" alt="s5" src="https://github.com/Dattax/genie-docs-2/assets/1408846/408b45d7-6ab5-4613-aba2-ab8148dacb35">
</p>
<p>6. It will take a minute to start the instance and then it’ll say “Connect” when ready. Click on Connect.</p>
<p>
<img width="1341" alt="s6" src="https://github.com/Dattax/genie-docs-2/assets/1408846/23f188a4-81a3-4b95-acbf-f4a70cf31a5c">
</p>

## Build Your Interface (No-Code Editor):

1. Open the app.jl.html file in your project. This is where you'll design your app's layout.
2. Select from 70+ UI components (buttons, text fields, charts, etc.) and drag them onto the page. The Genie Builder panel provides tools to customize the look, properties, and behaviors of each component.
3. To Run, on the Genie Builder panel, click "Start Server".
4. This will open a web browser where you can preview and interact with your app.

# How to Deploy Genie Apps on JuliaHub:

Within Genie Builder, click the "Launch to JuliaHub" button. It will: 
1. Create a new 'Application' in your JuliaHub workspace
2. Automatically package and upload your Genie app
In your JuliaHub workspace, open the newly created Application.
Choose your desired hosting plan (Free tier is available)
Adjust resources (CPU, memory) if needed
Set any necessary environment variables
Hit the "Launch" button!













## Other (Old)

The most important step is to first have a functioning Genie app.
The [Official Genie resources page](https://genieframework.com/) provides further details on the various tools available to assist in the development.

For this tutorial, we will start with an existing app `GenieAppTutorial` available [here](https://github.com/JuliaComputing/GenieAppTutorial).

To kickoff a new project, Genie provides various helper functions. `GenieAppTutorial` was initiated with:

```julia
using Genie
Genie.newapp("GenieAppTutorial")
Genie.newcontroller("dashboards")
```

`Genie.newapp("GenieAppTutorial")` here acts in a similar way to `Pkg.generate()`: it setups of new a Julia package and includes all the required scripts to get a functional app skeleton.

## Deploying on JuliaHub

Like for any other JuliaHub [custom application](@ref apps), making a new app requires to provide a path to a git repo that contains a Julia package in which a script `bin/main.jl` acts as an entry point.

Genie provides builtin support to directly generate a JuliaHub startup script:

```julia
Genie.Deploy.JuliaHub.mainjl()
```

When launching the app, a port has to be specified, which should be set at `8000` by default:

![genie-launch](genie-launch.png)

## App accessibility

Once the app is started, anyone can now access the newly deployed dashboard using the link appearing in the job status.

If REST API entry points were made available, they can also be accessed, for example from the browser:

![genie-API](genie-api-browser.png)

Or programmatically:

```julia
using HTTP
HTTP.get("http://APP-URL/api?n=120")
```

Here the endpoint simply returns the data from observation #`n`.

## Next steps

Congratulations on completing this tutorial! You now know how to run an interactive application powered by Genie on JuliaHub.
