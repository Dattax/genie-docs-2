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

<p>1. Once the Julia/Genie IDE opens, you'll need to wait a few minutes for Genie to start up. If it doesn't start, click on **GB stopped** at the bottom of the screen and it will then start the instance.</p>
<p>
<img width="1438" alt="g0" src="https://github.com/Dattax/genie-docs-2/assets/1408846/3b44094d-4fab-41fa-b6ad-69e246aeac0e">
</p>
<p>2. Once started, you should see a tab appear on the lower-left side of the screen that says **Genie**</p>
<p>
<img width="1437" alt="g1" src="https://github.com/Dattax/genie-docs-2/assets/1408846/7482afcb-2387-4612-af4e-ef4dc49fb490"> 
</p>
<p>3. This should start the drag n' drop functionalty of Genie Builder. If it doesn't click on the app.jl.html and it will open the
editor. On the right, you'll see components you can drag into the screen to build your application.</p>
<p><img width="1440" alt="g2" src="https://github.com/Dattax/genie-docs-2/assets/1408846/9c284d7c-24a6-45ea-938f-ec0fa253c561"></p>
<p>4. If you want to preview your app, click on the preview icon located on the bottom left. It may not appear until hover over.</p>
<p><img width="1440" alt="g3" src="https://github.com/Dattax/genie-docs-2/assets/1408846/1d11d864-bfcd-4bc6-a30b-1af44bf5df4a"></p>
<p>5. This is how the preview mode will look:  </p>
<p><img width="1440" alt="g4" src="https://github.com/Dattax/genie-docs-2/assets/1408846/7d2f9eb3-2be0-4622-b2a4-1f139175e079">
</p>

# How to Deploy Genie Apps on JuliaHub:

<p>1. Once you are done editing your Genie Builder app, you can launch it live on JuliaHub for the public or for just your organization to see. Go back to your project view.</p>
<p>2. If you are in collaborative edting mode, you will notice that the deploy button is greyed out. This is because in this editing mode, you can only deploy from the Source (main branch).</p>
<p><img width="1440" alt="f1" src="https://github.com/Dattax/genie-docs-2/assets/1408846/8d76225d-1cb1-4a39-8498-eb146726df89"></p>
<p>3. Before you switch to source, you should make sure your app changes in your workspace are published (committed) to the source branch. To do so, click on the publish button.</p>
<p>
<img width="1440" alt="f2" src="https://github.com/Dattax/genie-docs-2/assets/1408846/50b1f243-f12b-48a6-838d-f52fe1ce70fb"> 
</p>
<p>4. Now you can switch the source branch.</p>
<p><img width="1440" alt="f3" src="https://github.com/Dattax/genie-docs-2/assets/1408846/956927f9-47ce-4a4f-9b20-78634b77717f"></p>
<p>5. From the source (main branch) of the project, you can now deploy the project.</p>
<img width="1440" alt="f4" src="https://github.com/Dattax/genie-docs-2/assets/1408846/4b34319b-b005-4fab-ab5b-c1f957b8b752">
</p>
<p>6. The first time you do this, JuliaHub may ask for your credit card information. This is because deploying an app and hosting it costs money. You can learn more about our [pricing for hosted apps here](https://help.juliahub.com/juliahub/stable/tutorials/web_hosting/).</p>
<p>7. Once you have input your credit card information and returned to the project and hit deploy, the project will now ask you a few options for your hosted app. From here, you can select the size of the machine (hosting plan), the time limit for your app to be live, and the authorization type of totally public or just hosted for you or your organization. The most important thing to check here is that the port number is set to 9999. If not, please enter 9999. Then hit Start.</p>
<p><img width="1437" alt="f6" src="https://github.com/Dattax/genie-docs-2/assets/1408846/aad8c5db-8ee7-426f-ab9e-39a7d4edd032"></p>
<p>8. Now, the app will start the deployment process. It may take up to 5 minutes for your app to be deployed on the selected machine. Once ready, you can hit the Connect button to launch your live app. </p>
<p>
 <img width="1391" alt="f7" src="https://github.com/Dattax/genie-docs-2/assets/1408846/f331947b-dfcc-47d1-936b-f979d09feebb">
</p>
<p>9. Alternatively, you can selet on the right-hand arrow and click on the copy link button.</p>
<p>
<img width="1395" alt="f8" src="https://github.com/Dattax/genie-docs-2/assets/1408846/977615b4-57dc-4033-8b5a-791258a1a02d">
</p>
<p>10. This will give you the URL of your live app and options to embed this on other sites.</p>
<p>
<img width="1436" alt="f9" src="https://github.com/Dattax/genie-docs-2/assets/1408846/7d3d5f7d-df2e-4e43-9f0a-5be76265ff0f">
</p>
<p>11. Congratulations! You should see your live app at the URL on JuliaHub.</p>
<p>
<img width="1439" alt="f10" src="https://github.com/Dattax/genie-docs-2/assets/1408846/2f861115-071e-4224-a277-02188940fcbf"></p>

## Feedback

## Troubleshooting

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
