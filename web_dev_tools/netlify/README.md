# Netlify

#### Netlify CMS

Netlify CMS is the first CMS for the new age of Git-centric web development. It is completely build tool agnostic and works with storing structured content in Git. A CMS for site generators. Netlify CMS gives non-technical users a simple way to edit and add content to any site built with a site generator. [https://www.netlifycms.org](https://www.netlifycms.org/)

[Contribute on GitHub](https://github.com/netlify/netlify-cms)

#### Netlify Playground

Netlify Playground is a sandbox application to test all configurations related with Netlify before setting those up in your sites. [https://github.com/netlify/netlify-playground](https://github.com/netlify/netlify-playground)

[Contribute on GitHub](https://github.com/netlify/netlify-playground)

#### GoTell

GoTell is an API and build tool for handling large amounts of comments. [https://github.com/netlify/gotell](https://github.com/netlify/gotell)

[Contribute on GitHub](https://github.com/netlify/gotell)

#### GoTrue

GoTrue is a small open-source API written in golang that can act as a self-standing API service for handling user registration and authentication for projects. It's based on OAuth2 and JWT and will handle user signup, authentication and custom user data. [https://www.gotrueapi.org/](https://www.gotrueapi.org/)

[Contribute on GitHub](https://github.com/netlify/gotrue)

#### GoJoin

GoJoin is a tiny API that acts as a wrapper for Stripe's subscription API. It exposes simple call methods for single page apps and sites. [https://github.com/netlify/gojoin](https://github.com/netlify/gojoin)

[Contribute on GitHub](https://github.com/netlify/gojoin)

#### GoCommerce

GoCommerce is a small Go based API for e-commerce sites that handles orders and payments. It integrates with Stripe for payments and will support international pricing and VAT verification. [https://www.gocommerceapi.org/](https://www.gocommerceapi.org/)

[Contribute on GitHub](https://github.com/netlify/gocommerce)

#### Gotiator

A tiny API Gateway based on JSON Web Tokens. Gotiator can handle simple API proxying with signing for single page apps that already use JWTs for authentication. [https://github.com/netlify/gotiator](https://github.com/netlify/gotiator)

[Contribute on GitHub](https://github.com/netlify/gotiator)

### Open Source ❤️ Netlify

Many open source projects have found their home on Netlify.

#### Lodash

Lodash is a modern JavaScript utility library with more than half a billion downloads a year. [https://lodash.com](https://lodash.com/)

[Learn more](https://lodash.com/)

#### Yarn

Yarn is a fast, reliable, and secure dependency manager for node from the engineers at Facebook, Google and Microsoft. [https://yarnpkg.com](https://yarnpkg.com/)

[Learn more](https://yarnpkg.com/)

#### Serverless

Serverless is an application framework to easily build serverless architectures on AWS Lambda & more. [https://serverless.com](https://serverless.com/)

[Learn more](https://serverless.com/)

#### Framer.js

Framer.js is the most popular OS code design project out there. [https://framerjs.com](https://framerjs.com/)

[Learn more](https://framerjs.com/)

#### Kubernetes

Kubernetes is an open-source system for automating deployment, scaling, and management of containerized applications. [https://kubernetes.io](https://kubernetes.io/)

[Learn more](https://kubernetes.io/)

#### Your open source site on Netlify

Open source project teams qualify for free unlimited members.

[Find out more](https://www.netlify.com/legal/open-source-policy)

### Our Contributions

Netlify frequently contributes to many different projects in our space, in an effort to push the category forward.

#### Jekyll

Most popular static site generator, and first modern static site generator as well. [https://jekyllrb.com](https://jekyllrb.com/)

[Contribute on GitHub](https://github.com/jekyll/jekyll)

#### Roots

A toolkit for rapid advanced front-end development. [https://roots.netlify.com](https://roots.netlify.com/)

[Contribute on GitHub](https://github.com/jescalan/roots)

#### Hugo

A Fast and Flexible Static Site Generator built with love in Golang. [https://gohugo.io](https://gohugo.io/)

[Contribute on GitHub](https://github.com/spf13/hugo)

#### Apache Traffic Server

A fast, scalable and extensible caching proxy server. [http://trafficserver.apache.org](http://trafficserver.apache.org/)

[Contribute on GitHub](https://github.com/apache/trafficserver)

#### Middleman

Hand-crafted frontend development. [https://middlemanapp.com](https://middlemanapp.com/)

[Contribute on GitHub](https://github.com/middleman/middleman)

#### Docker

The open-source application container engine. [https://www.docker.com](https://www.docker.com/)

[Contribute on GitHub](https://github.com/docker/docker)

#### NATS

A simple, high performance open source messaging system for cloud native applications, IoT messaging, and microservices architectures. [http://nats.io](http://nats.io/)

[Contribute on GitHub](https://github.com/nats-io/nats)

#### Git2Go

Go bindings for libgit2. [https://github.com/libgit2/git2g](https://github.com/libgit2/git2g)

[Contribute on GitHub](https://github.com/libgit2/git2go)

#### Octokit

Ruby toolkit for the GitHub API. [http://octokit.github.io/octokit.rb](http://octokit.github.io/octokit.rb)

[Contribute on GitHub](https://github.com/octokit/octokit.rb)

#### Google Cloud Client Library for Ruby

Idiomatic Ruby client for Google Cloud Platform services. [https://github.com/GoogleCloudPlatform/google-cloud-ruby](https://github.com/GoogleCloudPlatform/google-cloud-ruby)

[Contribute on GitHub](https://github.com/GoogleCloudPlatform/google-cloud-ruby)

#### Boulder

An ACME-based CA, written in Go. [https://github.com/letsencrypt/boulder](https://github.com/letsencrypt/boulder)

[Contribute on GitHub](https://github.com/letsencrypt/boulder)

#### Lego

Let's Encrypt client and ACME library written in Go. [https://github.com/xenolf/lego](https://github.com/xenolf/lego)

[Contribute on GitHub](https://github.com/xenolf/lego)





## Site deploys overview

Netlify enforces a strict concept of atomic deploys. If you’re used to uploading files with FTP, SSH, RSync or S3’s API, this is quite a different concept.

Instead of pushing individual files to Netlify, you always create a new deploy. Netlify will compare the new deploy with your existing deploy and determine which files have changed and need to be uploaded.

No changes go live on your site’s public URL before all changes have been uploaded. Once all the changes are ready, the new version of the site immediately goes live on the CDN.

This means deploys are atomic, and your site is never in an inconsistent state while you’re uploading a new deploy.

With FTP or S3 uploads, each file is just pushed live one after the other, so you can easily get into situations where a new HTML page is live before the supporting assets \(images, scripts, CSS\) have been uploaded. And if your connection cuts out in the middle of an upload, your site could get stuck in a broken state for a long time.

Atomic deploys guarantee that your site is always consistent.

### [\#](https://docs.netlify.com/site-deploys/overview/#deploy-summary)Deploy summary <a id="deploy-summary"></a>

You can find a deploy summary on the detail page of any successful deploy, right above the [deploy log](https://docs.netlify.com/site-deploys/overview/#deploy-log). It allows you to quickly identify your deploy status and refer to the details in the log based on different types of information.

This summary indicates how many files have been uploaded to our CDN. It also indicates the status of site [headers](https://docs.netlify.com/routing/headers/), [redirects](https://docs.netlify.com/routing/redirects/), and [Edge Handlers](https://docs.netlify.com/edge-handlers/overview/) included in the deploy. It also indicates whether your site contains content served over insecure HTTP, known as [mixed content](https://developers.google.com/web/fundamentals/security/prevent-mixed-content/what-is-mixed-content).

When you have [branch deploys](https://docs.netlify.com/site-deploys/overview/#branch-deploy-controls) enabled, the summary will inform you if the files to upload have already been uploaded by a previous deploy with the same commits. Netlify’s deployment infrastructure knows how to avoid uploading the same file twice, even between different deploys, so we get your changes ready without duplicating content. You can read more about how this works in this article about our [deploying and routing infrastructure](https://medium.com/netlify/how-netlifys-deploying-and-routing-infrastructure-works-c90adbde3b8d).

If the summary continually indicates that many more files were uploaded than you were expecting, your site may be taking longer to deploy than it needs to. Visit our Forums for a verified Support Guide on [making the most of Netlify’s CDN cache](https://answers.netlify.com/t/common-issue-making-the-most-of-netlifys-cdn-cache/127) to learn about why this might be happening and get advice about what you can do to reduce the number of files uploaded each time in order to speed up your deploys.

### [\#](https://docs.netlify.com/site-deploys/overview/#deploy-log)Deploy log <a id="deploy-log"></a>

You can find a deploy log on the detail page of every deploy. The log provides content such as:

* details about your site’s build image, dependency caching, and Netlify Build process, including all of the standard output which comes from running your build
* information about any Build Plugins your site may have installed and their execution
* details about the success, failure, or cancellation of the deploy

For any successful deploy, highlights from the deploy log will be included in the [deploy summary](https://docs.netlify.com/site-deploys/overview/#deploy-summary). For failed deploys, visit our Forums for a verified Support Guide on [using the log to debug your build process](https://answers.netlify.com/t/common-issue-using-build-logs-to-debug-your-build-process/3067).

#### [\#](https://docs.netlify.com/site-deploys/overview/#share-log-content)Share log content <a id="share-log-content"></a>

Deploy logs for a site linked to a private repo are available to all site members. For a site linked to a public repo, you can control [deploy log visibility](https://docs.netlify.com/configure-builds/get-started/#definitions-1) to determine the privacy level.

To share deploy log content, you can copy the entire log by selecting **Copy to clipboard** \(the clipboard icon\). You can also generate a shareable URL for a single log line or a range of lines.

* For a single log line, select the line number to highlight the line.
* For a range of log lines, select the line number for the first log line in the range, then press shift and select the final log line number to highlight the full range.

  ![selected deploy log lines.](https://docs.netlify.com/images/site-deploys-deploy-log-selected-lines.png)

* If needed, press esc to deselect log lines.

Once you’ve selected a line or range, copy the resulting URL from the address bar of your web browser. The URL syntax should resemble this: `https://app.netlify.com/sites/SITE_NAME/deploys/DEPLOY_ID#L5-L10`

### [\#](https://docs.netlify.com/site-deploys/overview/#branches-and-deploys)Branches and deploys <a id="branches-and-deploys"></a>

Netlify lets you control which branches in your Git repository you want to deploy.

#### [\#](https://docs.netlify.com/site-deploys/overview/#definitions)Definitions <a id="definitions"></a>

* **Production branch**: the Git branch that Netlify uses to build and deploy changes to your site’s main URL. For example, `www.yourcustomdomain.com` and `yoursitename.netlify.app`.
* **Production deploy**: a deploy from the production branch. If auto publishing is enabled, each new production deploy will update what is published at your site’s main URL.
* **Branch deploy**: a deploy generated from a branch that is not your production branch. Branch deploys are published to a URL which includes the branch name as a prefix. For example, if a branch is called `staging`, it will deploy to `staging--yoursitename.netlify.app`. If you use Netlify DNS, you can enable branch subdomains, so the `staging` branch example would deploy to `staging.yourcustomdomain.com`.
* **Deploy Preview**: a deploy generated from a pull request or merge request, building the site as it would be if the proposed changes were merged. Deploy Previews are published to a URL which has the prefix `deploy-preview` followed by the identifier number of the pull request or merge request. For example, a Deploy Preview for pull/merge request \#42 will deploy to `deploy-preview-42--yoursitename.netlify.app`. For more information, visit the docs on [Deploy Previews](https://docs.netlify.com/site-deploys/deploy-previews/).
* **Permalink**: every successful build of your site also creates a deploy permalink that starts with the deploy ID number. For example: `1234abcd12acde000111cdef--yoursitename.netlify.app`. The web content at this URL never changes. This is in contrast to production deploys, branch deploys, and Deploy Previews where the web content is updated when you merge or push new commits.

#### [\#](https://docs.netlify.com/site-deploys/overview/#branch-deploy-controls)Branch deploy controls <a id="branch-deploy-controls"></a>

By default, Netlify deploys the site’s production branch after every change.

To generate branch deploys for other branches in your repository, select your site on the **Sites** page. Then go to **Site settings &gt; Build & deploy &gt; Continuous Deployment &gt; Branches**, and select **Edit settings**. You can choose to deploy all branches \(including future branches\), or select individual branches you would like to deploy.

![undefined](https://docs.netlify.com/images/site-deploys-allowed_branches.png)

When selecting individual branches for deployment, type the name of each branch you want to deploy. You can also enter branch names you haven’t created yet.

Once you select some or all of your branches for branch deploys, Netlify will start watching those branches for new commits and pull/merge requests. As soon as you start pushing changes to those branches, you’ll find new deploys for those branches.

#### [\#](https://docs.netlify.com/site-deploys/overview/#deploy-preview-controls)Deploy Preview controls <a id="deploy-preview-controls"></a>

By default, Netlify automatically builds Deploy Previews for GitHub pull requests and GitLab merge requests when the base/target branch is your production branch. If you enable branch deploys for some or all of your other branches, we’ll also build Deploy Previews for pull/merge requests against those branches. Collaboration tools available in the [Netlify Drawer](https://docs.netlify.com/site-deploys/deploy-previews/#collaborative-deploy-previews) are enabled by default for Deploy Previews.

You can control in the UI whether or not Deploy Previews are generated for pull/merge requests. You can also enable or disable the Netlify Drawer. To change these settings, select your site and go to **Site settings &gt; Build & deploy &gt; Continuous Deployment &gt; Deploy Previews**, then select **Edit settings**.

#### [\#](https://docs.netlify.com/site-deploys/overview/#search-engine-indexing)Search engine indexing <a id="search-engine-indexing"></a>

Netlify automatically ensures that only your currently published production deploy and most recent branch deploys can be indexed by search engines. Requests to Deploy Previews, unpublished production deploys, and old branch deploys will have an `X-Robots-Tag: noindex` header included in the response. Depending on how you use branch deploys, you may want to prevent even your most recent branch deploys from being indexed by search engines. You can do so by configuring [custom headers](https://docs.netlify.com/routing/headers/) in your branch.

### [\#](https://docs.netlify.com/site-deploys/overview/#deploy-contexts)Deploy contexts <a id="deploy-contexts"></a>

Deploy contexts give you the flexibility to [configure your site’s builds](https://docs.netlify.com/configure-builds/file-based-configuration/) depending on the context they are going to be deployed to.

There are three predefined deploy contexts:

* `production`: this context corresponds to the main site’s deployment, attached to the Git branch you set when the site is created.
* `deploy-preview`: this context corresponds to the previews we build for pull/merge requests.
* `branch-deploy`: this context corresponds to deploys from branches that are not the site’s main production branch.

Besides these three predefined contexts, sites can use also branch names as custom deploy contexts. For example, a branch called `staging` will match a deploy context called `staging`.

Deploy contexts allow you to override options from your site’s settings including the build command, the environment variables added to the build, [Build Plugin configuration](https://docs.netlify.com/configure-builds/build-plugins/#configure-by-deploy-context), and more.

Overrides are applied in a hierarchical order. The site’s global settings apply to each deploy, if we’re building the production site, and if you change options in your production context, they will be overridden. Only options that are set explicitly are overridden; if you leave one out, the build will use the value of the global settings or previous contexts. Environment variables are also overridden individually, for example, you can have access tokens as environment variables per context.

To configure deploy contexts, you must create a file called `netlify.toml` in the root of your Git repository. There, you can set as many contexts as you want to configure.

```text
# Production context:
# All deploys from the main repository branch
# will inherit these settings.
[context.production]
  command = "make production"
  [context.production.environment]
    ACCESS_TOKEN = "super secret"
  # Deploys from main branch run this plugin in the build.
  # Plugins context requires double brackets.
  [[context.production.plugins]]
    package = "@netlify/plugin-sitemap"

# Deploy Preview context:
# All deploys generated from a pull/merge request
# will inherit these settings.
[context.deploy-preview.environment]
  ACCESS_TOKEN = "not so secret"

# Branch deploy context:
# All deploys that are not from a pull/merge request
# or from the production branch will inherit these settings.
[context.branch-deploy]
  command = "make staging"

# Specific branch context:
# Deploys from this branch will take these settings
# and override their current ones.
[context.feature]
  command = "make feature"

[context."features/branch"]
  command = "gulp"
```

File-based configuration settings will override those set in the UI. In the `netlify.toml` file, settings for more specific contexts will override more general ones. For example, settings for a specific branch will override those for branch-deploy.

Visit our docs on [file-based configuration](https://docs.netlify.com/configure-builds/file-based-configuration/) to learn more about what you can do with deploy contexts.

### [\#](https://docs.netlify.com/site-deploys/overview/#more-site-deploys-resources)More site deploys resources <a id="more-site-deploys-resources"></a>

* [Create deploys](https://docs.netlify.com/site-deploys/create-deploys/)
* [Manage deploys](https://docs.netlify.com/site-deploys/manage-deploys/)
* [Deploy Previews](https://docs.netlify.com/site-deploys/deploy-previews/)
* [Split Testing](https://docs.netlify.com/site-deploys/split-testing/)
* [Deploy notifications](https://docs.netlify.com/site-deploys/notifications/)
* [Post processing](https://docs.netlify.com/site-deploys/post-processing/)



## Create deploys

This page covers features and tools you can use to create deploys with or without continuous deployment.

Note

When you create a deploy manually without continuous deployment, Netlify does not run a build command.

### [\#](https://docs.netlify.com/site-deploys/create-deploys/#deploy-with-git)Deploy with Git <a id="deploy-with-git"></a>

Continuous deployment works by [connecting a Git repository to a Netlify site](https://docs.netlify.com/configure-builds/get-started/) and keeping the two in sync.

It works for plain static sites, but it’s even more powerful when you’re using a [static site generator](https://www.staticgen.com/) or a frontend build tool like [webpack](https://webpack.js.org/), [Gulp](http://gulpjs.com/), or [Grunt](http://gruntjs.com/).

Netlify will run your build command and deploy the result whenever you push to your Git repo. The benefits of Netlify’s continuous deployment include:

* No deploying without committing and pushing first
* Easy collaboration through pull/merge requests
* Fix a typo through your Git provider’s web UI from your mobile
* Edit content without code by using a static site CMS, [Netlify CMS](https://netlifycms.org/)

### [\#](https://docs.netlify.com/site-deploys/create-deploys/#netlify-cli)Netlify CLI <a id="netlify-cli"></a>

You can use the CLI to [set up continuous deployment](https://docs.netlify.com/cli/get-started/#continuous-deployment) for a Git repository. You can also use the CLI to [create manual deploys](https://docs.netlify.com/cli/get-started/#manual-deploys) without continuous deployment.

### [\#](https://docs.netlify.com/site-deploys/create-deploys/#drag-and-drop)Drag and drop <a id="drag-and-drop"></a>

You can create a new site by dragging a project folder to the deploy dropzone in [Netlify Drop](https://app.netlify.com/drop) or at the bottom of **Sites**. If your site is not connected to a Git repository, you can deploy your site manually by using the deploy dropzone at the bottom of the **Deploys** page. For teams without sites, a deploy dropzone will also appear in **Team overview**.

### [\#](https://docs.netlify.com/site-deploys/create-deploys/#api-endpoints)API endpoints <a id="api-endpoints"></a>

You can use the [API](https://docs.netlify.com/api/get-started/#deploy-via-api) to create deploys manually using a file digest or a zip file.

### [\#](https://docs.netlify.com/site-deploys/create-deploys/#deploy-to-netlify-button)Deploy to Netlify button <a id="deploy-to-netlify-button"></a>

The **Deploy to Netlify** button helps users deploy new sites from templates with one single click. It provides web developers a simple one-click step to let their users deploy those applications on Netlify.

It’s designed to be used in README files, documentation sites, and probably anything that renders as an html file.

This is an example of how it looks:[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/netlify/netlify-statuskit)

The template code must be available in a public repository stored on GitHub.com or GitLab.com.

#### [\#](https://docs.netlify.com/site-deploys/create-deploys/#markup)Markup <a id="markup"></a>

You can use any markup language that renders as HTML to display the button. There are two very important URLs that you’ll need:

* The SVG URL for the button: `https://www.netlify.com/img/deploy/button.svg`.
* The URL the button takes users to: `https://app.netlify.com/start/deploy`. This link requires the public Git repository as a parameter, for example:

  ```text
  https://app.netlify.com/start/deploy?repository=https://github.com/netlify/netlify-statuskit
  ```

#### [\#](https://docs.netlify.com/site-deploys/create-deploys/#template-configuration)Template configuration <a id="template-configuration"></a>

You can provide a set of default values for your template directly in the template’s git repository. Create a `netlify.toml` file in the root of the repository, if you don’t have it already. We’ll read the information from there. This file can also be used to set options for continuous deployment, you can read more about it in the [file-based configuration documentation](https://docs.netlify.com/configure-builds/file-based-configuration/).

Within the `[template]` section in that file, you can set two directives:

* A list of incoming hooks for the users site. This is very useful if you want to allow a third party service to control when to deploy the site. This is what headless CMS services like Contentful and DatoCMS do. Users can give those providers the address Netlify generates for their specific incoming requests.

  ```text
  [template]
    incoming-hooks = ["Contentful"]
  ```

* A list of required environment variables. This is the way to let users configure specific configuration options upon deployment. It also enables customization without having to change the code of the base template.

  ```text
  [template.environment]
    SECRET_TOKEN = "change me for your secret token"
    CUSTOM_LOGO = "set the url to your custom logo here"
  ```

#### [\#](https://docs.netlify.com/site-deploys/create-deploys/#pre-fill-environment-variables)Pre-fill environment variables <a id="pre-fill-environment-variables"></a>

You can pass environment variable values for the site template in the hash of the template’s Deploy to Netlify URL with key/value pairs. Using the example environment variables above, `SECRET_TOKEN` and `CUSTOM_LOGO`, the resulting URL will be something like this:

```text
https://app.netlify.com/start/deploy?repository=https://github.com/myworkspace/sweetkittentemplate#SECRET_TOKEN=specialuniquevalue&CUSTOM_LOGO=https://placekitten.com/100/100
```

Passing environment variable values in the hash ensures that they’re processed on the client side only. You can can create custom Deploy to Netlify buttons for your users with tokens and other secure data, and they won’t appear in Netlify logs.

### [\#](https://docs.netlify.com/site-deploys/create-deploys/#build-hooks)Build hooks <a id="build-hooks"></a>

[Build hooks](https://docs.netlify.com/configure-builds/build-hooks/) give you unique URLs you can use to trigger new builds and deploys.

### [\#](https://docs.netlify.com/site-deploys/create-deploys/#zapier-integrations)Zapier integrations <a id="zapier-integrations"></a>

Netlify is available on Zapier, where you can connect Netlify with over 1,000 other applications. You can use Zapier “Zaps” to start a new deploy of your site in response to a trigger from another service. You can [find out more on our blog](https://www.netlify.com/blog/2018/11/07/automate-your-netlify-sites-with-zapier/), or use one of the templates below to get started:Start deploys of Netlify sites daily[Use this Zap](https://zapier.com/apps/netlify/integrations/schedule/29330/start-deploys-of-netlify-sites-daily?utm_source=widget&utm_medium=embed&utm_campaign=Widget)Start Netlify deploys when you send new Tweets[Use this Zap](https://zapier.com/apps/netlify/integrations/twitter/29745/start-netlify-deploys-when-you-send-new-tweets?utm_source=widget&utm_medium=embed&utm_campaign=Widget)Start Netlify site deploys with the push of a Flic button[Use this Zap](https://zapier.com/apps/flic/integrations/netlify/29780/start-netlify-site-deploys-with-the-push-of-a-flic-button?utm_source=widget&utm_medium=embed&utm_campaign=Widget)See more [Netlify](https://zapier.com/apps/netlify/integrations?utm_medium=partner_api&utm_source=widget&utm_campaign=Widget) integrations powered by![](https://zapier.com/apps/app-event-tracker?utm_source=widget&utm_medium=embed&utm_campaign=Widget)

#### Did you find this doc useful?



## Deploy Previews

Deploy Previews allow you and your team to experience changes to any part of your site without having to publish them to production.

Netlify builds Deploy Previews by default for GitHub pull requests and GitLab merge requests. You can control whether or not Deploy Previews are generated for pull/merge requests. For more information, visit the [Deploy Preview controls](https://docs.netlify.com/site-deploys/overview/#deploy-preview-controls) docs.

For successful deploys, your pull/merge request comments include a link to the Deploy Preview by default. You can add, remove, or edit these notifications. Visit the [deploy notifications](https://docs.netlify.com/site-deploys/notifications/) doc for more information.

### [\#](https://docs.netlify.com/site-deploys/deploy-previews/#deploy-preview-urls)Deploy Preview URLs <a id="deploy-preview-urls"></a>

Deploy Previews work by deploying pull/merge requests to a unique URL different from the one your production site uses. This URL has the prefix `deploy-preview` followed by the identifier number of the pull request or merge request. For example, a Deploy Preview for pull/merge request \#42 will deploy to `deploy-preview-42--yoursitename.netlify.app`. The web content of this URL is updated every time changes are pushed to the associated pull/merge request.

You can share this URL with your team to collaborate and [gather feedback](https://docs.netlify.com/site-deploys/deploy-previews/#get-feedback).

Every deploy also has a permalink that starts with the deploy ID number. For example: `1234abcd12acde000111cdef--yoursitename.netlify.app`. The contents of this URL never change, even after you redeploy your site.

### [\#](https://docs.netlify.com/site-deploys/deploy-previews/#collaborative-deploy-previews)Collaborative Deploy Previews <a id="collaborative-deploy-previews"></a>

With collaborative Deploy Previews, you and your team can add, review, and manage feedback about site changes right from your site. You can leave comments, take screenshots and video, and test responsiveness on a mobile device.

You can access collaboration tools in the Netlify Drawer using the Netlify icon in your Deploy Preview.

![Netlify Drawer icon](https://docs.netlify.com/images/site-deploys-deploy-previews-netlify-drawer.png)

#### [\#](https://docs.netlify.com/site-deploys/deploy-previews/#requirements-and-limitations)Requirements and limitations <a id="requirements-and-limitations"></a>

Keep the following considerations in mind when working with collaborative Deploy Previews.

**\#Requirements**

* **Deploy Preview URLs**. Collaboration tools are only available on Deploy Previews accessed through their `deploy-preview` prefixed URLs.
* **GitHub app permissions**. If you’re using GitHub, verify that the Netlify GitHub app is [installed with the necessary permissions](https://docs.netlify.com/configure-builds/repo-permissions-linking/#authentication-with-the-netlify-github-app).
* **Valid HTML**. Your site must have valid HTML output with opening and closing `body` tags.
* **Team access**. Stakeholders must be signed into Netlify and [granted access](https://docs.netlify.com/accounts-and-billing/team-management/manage-team-members) to a team to use the collaboration tools. To request access to collaborate, select the **Team Members** tab and select **Request to join team**.

**\#Limitations**

* **On-demand Builders and server-side rendering**. Collaboration tools are not available on sites using On-demand Builders or server-side rendering.
* **Bitbucket**. Collaboration tools are currently not available on Bitbucket deploys.

#### [\#](https://docs.netlify.com/site-deploys/deploy-previews/#give-feedback)Give feedback <a id="give-feedback"></a>

The Netlify Drawer provides access to a number of collaboration tools that team members and approved Reviewers can use to leave feedback about a Deploy Preview.

**\#Leave comments**

Team members and approved Reviewers can leave comments on the Deploy Preview that are synced and mirrored on the GitHub pull request or GitLab merge request. Select the **Activity** tab in the Netlify Drawer to start writing a comment.

If you are a pending Reviewer, your submitted comments will remain hidden until a team Owner or Collaborator approves you.

**\#Send feedback to third-party services**

You can send feedback about a Deploy Preview to a number of productivity tools by connecting your Netlify user account to your user account for the tool:

* [GitHub](https://github.com/)
* [GitLab](https://gitlab.com/)
* [Jira Software](https://www.atlassian.com/software/jira) \(may not be available on all [plans](https://www.netlify.com/pricing/)\)
* [Shortcut](https://shortcut.com/)
* [Linear](https://linear.app/)
* [Trello](https://trello.com/)

To get started, go to the **Integrations** tab in the Netlify Drawer and select **Connect** for the third-party service you want to use.

![Netlify Drawer Integrations tab](https://docs.netlify.com/images/site-deploys-deploy-previews-integrations.png)

Once your Netlify user account is connected to a third-party service, you can submit feedback to the service directly from the Deploy Preview by selecting **New issue**.

**\#Take screenshots and record screen**

You can take a screenshot or screen recording and use it in feedback in the pull/merge request or third-party integration.

To add a screenshot, hover over the Netlify icon and select **Take screenshot**. You can edit and annotate your screenshot before using it in feedback.

To record a screen interaction, hover over the Netlify icon and select **Record screen**. You can use the screen recording in your feedback as a GIF.

You can also drag and drop image and video files directly onto the **Activity tab** text area to include them in a comment using Markdown syntax.

#### [\#](https://docs.netlify.com/site-deploys/deploy-previews/#get-feedback)Get feedback <a id="get-feedback"></a>

The Netlify Drawer also provides tools for team Owners and Collaborators to request feedback about a Deploy Preview.

**\#Invite contributors**

You can select **Add members** to invite users to join your team, including an unlimited number of free Reviewers.

For more information on team member permissions, check the [team roles](https://docs.netlify.com/accounts-and-billing/team-management/manage-team-members/#team-roles) documentation.

**\#Set entry path**

The entry path is the page visitors will land on when they access your Deploy Preview using links on the **Deploys** page, deploy details page, in GitHub, or in GitLab. You can set an entry path in the following ways:

* Enter the path in the **Settings** tab of the Netlify Drawer.
* Tag `@netlify /path/to/page` in the initial description of your GitHub pull request or GitLab merge request.
* Hover over the Netlify icon and select **Set as entry path** to save the current page as the initial route. This option only appears if you are the author of the pull/merge request.

When writing a value for the entry path, it must be relative and start with `/`.

#### [\#](https://docs.netlify.com/site-deploys/deploy-previews/#test-and-troubleshoot-with-collaboration-tools)Test and troubleshoot with collaboration tools <a id="test-and-troubleshoot-with-collaboration-tools"></a>

The Netlify Drawer provides access to tools that team Owners, Collaborators, and Reviewers can use to test and troubleshoot specific site deploys.

**\#Monitor logs**

Owners and Collaborators can access the deploy log and serverless function logs in the Netlify Drawer to help with monitoring and troubleshooting a specific deploy.

To find details about the deploy, open the **Deploy Logs** tab of the Netlify Drawer. Visit our [deploy log docs](https://docs.netlify.com/site-deploys/overview/#deploy-log) for more information.

You can access serverless function logs by opening the **Function logs** tab in the Netlify Drawer and selecting a function to check out its latest log contents for the current session. Visit our [Function logs docs](https://docs.netlify.com/functions/logs/) for more information.

**\#Check responsiveness and site performance**

You can open your Deploy Preview on your mobile device to check your site’s performance and test responsiveness. To open your Deploy Preview on a mobile device, hover over the Netlify icon and select **Open on device**. You can then scan the QR code with your device to open the page.

**\#Access browser details and replicate in BrowserStack**

When someone shares feedback through a collaborative Deploy Preview, you can access metadata about the browser the comment author used. You can also replicate their browser environment for testing and QA through a built-in integration with [BrowserStack](https://www.browserstack.com/).

In collaborative Deploy Preview feedback, find the browser information \(usually near the bottom of the feedback\) and select **Open in BrowserStack** to launch a BrowserStack instance that matches the author of the comment’s browser, browser version, viewport size, and operating system.

The BrowserStack service provides a free [60 minute total usage allotment](https://www.netlify.com/blog/2021/07/20/troubleshoot-qa-issues-faster-with-browserstack-and-deploy-previews/#extended-free-browserstack-minutes-for-netlify-users) for users who sign up from Netlify. An option to upgrade is available in BrowserStack once the allotment is finished.

#### [\#](https://docs.netlify.com/site-deploys/deploy-previews/#troubleshooting-collaborative-deploy-previews)Troubleshooting collaborative Deploy Previews <a id="troubleshooting-collaborative-deploy-previews"></a>

This section provides troubleshooting tips for using and accessing collaborative Deploy Previews. Make sure you have reviewed the [requirements](https://docs.netlify.com/site-deploys/deploy-previews/#requirements) and [limitations](https://docs.netlify.com/site-deploys/deploy-previews/#limitations) for collaborative Deploy Previews before you begin.

If you have additional concerns that aren’t answered here, you can visit our [Forums](https://answers.netlify.com/categories) to ask questions and find more information.

**\#Netlify Drawer is missing**

If you can’t find the Netlify Drawer on your Deploy Preview, verify that the Netlify Drawer is enabled for your site. You can do this by going to your site in the Netlify UI and selecting **Site settings &gt; Build & deploy &gt; Continuous Deployment &gt; Deploy Previews**.

The Netlify Drawer also might not appear if your site’s [custom headers](https://docs.netlify.com/routing/headers/) include the following Content Security Policy \(CSP\) directives:

* `default-src`
* `script-src`
* `frame-src`
* `child-src`

To address this issue, add `app.netlify.com` and `netlify-cdp-loader.netlify.app` to the allow list in the `_headers` or `netlify.toml` file. For example:

* \_headers
* netlify.toml

```text
/* 
  Content-Security-Policy: child-src 'self' app.netlify.com; script-src 'self' app.netlify.com netlify-cdp-loader.netlify.app;
```

**\#Netlify Drawer blocks content**

If the Netlify Drawer is blocking important UI elements, you can drag and drop the icon and pin it to any of the four corners of your screen.

**\#Reviewer comments appear as a different GitLab user**

If a Reviewer authenticates with GitLab, comments they add through collaboration tools in a Deploy Preview are mirrored in a merge request using their GitLab profile. If a Reviewer doesn’t authenticate with GitLab or doesn’t have a GitLab account, comments mirrored in a merge request appear under the profile of the GitLab user who configured the site on Netlify. These mirrored comments start with **A reviewer left a comment**.

To change the GitLab user for unauthenticated comments on merge requests, a GitLab project Owner or Maintainer can take these steps:

1. In GitLab, invite a new user with a role of Reporter or above to your project. The email address for this user must be one you have access to.
2. Confirm the user and log into GitLab with that account.
3. Edit the [GitLab profile](https://gitlab.com/-/profile) of the user to change the **Full name** and **Public avatar**. We recommend naming the user `Netlify` and using the Netlify logo as the avatar to help associate unauthenticated comments with Netlify.
4. Generate a [personal access token](https://gitlab.com/-/profile/personal_access_tokens) with an `api` scope, and copy the token to your clipboard.
5. In a Deploy Preview from one of your GitLab sites, open the **Deploy settings** tab in the Netlify Drawer. Paste in the token from GitLab, and select **Save**.

   Comments left by Reviewers who have not authenticated with GitLab should now be associated with the Netlify user on your project.

**\#Preview changes without the Netlify Drawer**

To opt out of loading the Netlify Drawer on a site’s Deploy Previews, go to **Site settings &gt; Build & deploy &gt; Continuous Deployment &gt; Deploy Previews**, select **Edit settings**, and disable the Netlify Drawer.

You can also open a [branch deploy or deploy permalink](https://docs.netlify.com/site-deploys/overview/#definitions) if you need to preview a deploy but don’t want to access any of the collaboration features. Both links are available in the Netlify Drawer under **Settings**. The branch deploy link is also available on your site’s **Deploys** page in the Netlify UI, while the deploy permalink is available on the deploy details page.



## Post processing

Netlify offers several post processing features to help you optimize your sites. These are available under **Site settings &gt; Build & deploy &gt; Post processing**.

### [\#](https://docs.netlify.com/site-deploys/post-processing/#post-processing-features)Post processing features <a id="post-processing-features"></a>

**Snippet injection** - Analytics or other scripts can be added to the HTML of your site using [snippet injection](https://docs.netlify.com/site-deploys/post-processing/snippet-injection/).

**Asset optimization** - You can rewrite link URLs to pretty URLs, bundle and minify CSS and JS, and compress images. These options can be controlled via [file-based configuration](https://docs.netlify.com/configure-builds/file-based-configuration/#post-processing) as well as in **Site settings**.

**Prerendering** - To allow search engines and social networks to crawl the pages rendered by your app, you can enable [prerendering](https://docs.netlify.com/site-deploys/post-processing/prerendering/).

**Form detection** - By default, Netlify scans new and updated HTML files to detect forms and set them up for receiving submissions. You can disable [form detection](https://docs.netlify.com/site-deploys/post-processing/form-detection/) to speed up deploys if you’re not using Forms.





## Snippet injection

Often you want to inject JavaScript snippets into all pages of your site, either in the `<head>` or at the end of the `<body>` tag.

Most analytics providers, retargeting services, and A/B testing services will give you an HTML snippet and ask you to add it to every page on your site. Netlify lets you do this without having to pollute the source code for the site with production specific analytics snippets.

You can pick between injecting the scripts before the closing `</head>` tag or before the closing `</body>` tag.

Note

Injected snippets will also show up on the `password` protection screen. This means you can verify that your analytics scripts are correctly configured without having to remove the password when your site is still under development.

### [\#](https://docs.netlify.com/site-deploys/post-processing/snippet-injection/#snippet-injection-ui)Snippet injection UI <a id="snippet-injection-ui"></a>

In **Site settings &gt; Build & Deploy &gt; Post processing**, find the **Snippet Injection** section and select **Add Snippet**. Then give your script a name and paste the script body \(including any `<script>` tags, etc\).

### [\#](https://docs.netlify.com/site-deploys/post-processing/snippet-injection/#api-endpoints)API endpoints <a id="api-endpoints"></a>

You can use the [API](https://docs.netlify.com/api/get-started/#snippets) to get snippets, add snippets, and more.

### [\#](https://docs.netlify.com/site-deploys/post-processing/snippet-injection/#more-resources)More resources <a id="more-resources"></a>

Explore snippet injection examples in our blog:

* [Promoting open source with Netlify snippet injection](https://www.netlify.com/blog/2018/09/06/promoting-open-source-with-netlify-snippet-injection/)
* [Add web monetization to your sites with snippet injection](https://www.netlify.com/blog/2020/12/14/add-web-monetization-to-your-sites-with-snippet-injection/)

## Prerendering

_This feature is in_ `BETA`.

If you’re using a single-page app for a site that’s not behind a login, SEO is an important concern.

Google, Bing, Yandex and other search engines and crawlers support Google’s [standard for Ajax Crawling](https://developers.google.com/webmasters/ajax-crawling/docs/specification).

Normally Google will penalize sites heavily for using “cloaking”, meaning showing different content to Google than to normal web visitors, but for single page apps they have an exception. When detecting a single page app their crawler will send an `_escaped_fragment_` query parameter in the request, and the origin server can then choose to return a document that represents the content a user will actually get when the single page app is running.

Note

Google has marked their Standard for Ajax Crawling as deprecated. They’re still following the standard, but recommend that single page app authors just rely on Google’s built-in capacity for interpreting JavaScript applications. In our experience that’s often still not enough and prerendering is often still a necessity.

### [\#](https://docs.netlify.com/site-deploys/post-processing/prerendering/#set-up-prerendering)Set up prerendering <a id="set-up-prerendering"></a>

Netlify comes with built-in prerendering. You can enable it for your site at **Site settings &gt; Build & deploy &gt; Post processing &gt; Prerendering**.

![Enabling Netlify&#x2019;s built-in prerendering](https://docs.netlify.com/images/site-deploys-prerendering.png)

Our built-in prerendering service will cache prerendered pages for between 24 and 48 hours; this is not adjustable.

#### [\#](https://docs.netlify.com/site-deploys/post-processing/prerendering/#external-services)External services <a id="external-services"></a>

_This feature may not be available on all_ [_plans_](https://www.netlify.com/pricing/)_._

You can also use external services that can automate prerendering for you:

* [Prerender.io](https://prerender.io/)
* [Brombone](http://www.brombone.com/)
* [Prerender.cloud](https://prerender.cloud/)

Prerender.io has an open-source version of their service that you can self-host.

If you want to use an external service, send us an email at [support@netlify.com](mailto:support@netlify.com) to let us know which service you’re using and its API token, and we’ll get you set up.

### [\#](https://docs.netlify.com/site-deploys/post-processing/prerendering/#how-it-works)How it works <a id="how-it-works"></a>

We’ve taken great care to implement support for prerendering in the most efficient manner possible.

When a request hits one of our CDN servers, our CDN software determines if it’s a prerendering request from a crawler. If prerendering is enabled for your site, our cache servers will contact the prerendering backend straight from our CDN nodes instead of serving the normal cached request.

If you’ve worked with Netlify support to configure an external service and the external prerendering backend makes good use of HTTP caching headers like max-age, ETags or Last-Modified dates, prerendered responses will be cached sensibly on our CDN edge nodes. In our initial tests we’ve seen average response times of ~100 ms to crawlers, which is low enough that Google will still give your site a SEO boost for being fast.

Visit our Support Forums to ask questions about [understanding and debugging prerendering](https://answers.netlify.com/t/common-issue-understanding-and-debugging-prerendering/150/2).



## Form detection

Netlify’s serverless form handling allows you to manage [forms](https://docs.netlify.com/forms/setup/) without extra API calls or additional JavaScript. The built-in form detection feature allows our build bots to automatically parse your HTML at deploy time.

### [\#](https://docs.netlify.com/site-deploys/post-processing/form-detection/#disable-form-detection)Disable form detection <a id="disable-form-detection"></a>

Although form detection is enabled by default, you may want to disable it if your site doesn’t have forms or you’re not using Netlify to manage them. Disabling form detection will reduce post processing and may speed up deploys.

To disable form detection for your site, go to **Site settings &gt; Build & deploy &gt; Post processing &gt; Form detection**, and select **Edit Settings**. Then clear the **Run Form detection** check box, and select **Save**.

At your next site deploy, Netlify build bots will no longer parse new or updated HTML files for forms. [Form submission](https://docs.netlify.com/forms/submissions/#form-submissions-ui) handling will be deactivated for any new or updated forms.

Warning

Disabling form detection is intended only for sites that don’t use Netlify Forms. If your site does use Netlify Forms, we recommend removing forms from your site code or altering your code to handle submissions by other means before disabling form detection.

### [\#](https://docs.netlify.com/site-deploys/post-processing/form-detection/#re-enable-form-detection)Re-enable form detection <a id="re-enable-form-detection"></a>

To enable form detection after disabling it, go to **Site settings &gt; Build & deploy &gt; Post processing &gt; Form detection**, and select **Edit Settings**. Then select **Run Form detection**, and select **Save**.

At your next site deploy, Netlify build bots will parse HTML to detect forms, and verified form submissions will be available on Netlify.

