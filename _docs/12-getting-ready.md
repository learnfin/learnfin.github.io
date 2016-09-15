---
title: "Getting Ready"
permalink: /docs/getting-ready/
excerpt: "Installing and loading uslfin R package."
modified: 2016-09-14T18:01:00-01:00
---

{% include base_path %}

You need the R client version 3.3.1 or higher. **You can download R from [here](https://cran.r-project.org/).** Click one of the "Download R for..." links suitable for your operating system (Mac, Windows or Linux) and install.
{: .notice--info}

Once you install R, rest of the installation is very easy. Just copy paste the code below to your R console. More experienced R users can examine the code and use what is strictly necessary.

{% gist 6df145c579806799122c492465c2ffde getting_ready_uslfin.r %}

That's it. Were you expecting more steps to install?

Even though it is unlikely, there is always a possibility that `uslfin` package will not install or one of the commands will go awkward. If that is the case, please make sure your R version is 3.3.1 or later. Second, restart R and even your machine. Finally, please notify me. (TODO: Put contact information.)
{: .notice--danger}

<!--
Minimal Mistakes has been developed to be 100% compatible with hosting a site on [GitHub Pages](https://pages.github.com/). To get up and running with a new GitHub repository quickly, follow these steps or jump ahead to the [full installation guide]({{ base_path }}/docs/installation/).

## Fork the Theme

Fork the [Minimal Mistakes theme](https://github.com/mmistakes/minimal-mistakes/fork), then rename the repo to **USERNAME.github.io** --- replacing **USERNAME** with your GitHub username.

<figure>
  <img src="{{ base_path }}/images/mm-theme-fork-repo.png" alt="fork Minimal Mistakes">
</figure>

**Note:** Your Jekyll site should be viewable immediately at <http://USERNAME.github.io>. If it's not, you can force a rebuild by **Customizing Your Site** (see below for more details).
{: .notice--warning}

If you're hosting several Jekyll based sites under the same GitHub username you will have to use Project Pages instead of User Pages. Essentially you rename the repo to something other than **USERNAME.github.io** and create a `gh-pages` branch off of `master`. For more details on how to set things up check [GitHub's documentation](https://help.github.com/articles/user-organization-and-project-pages/).

<figure>
  <img src="{{ base_path }}/images/mm-gh-pages.gif" alt="creating a new branch on GitHub">
</figure>

**ProTip:** Be sure to [delete](https://github.com/blog/1377-create-and-delete-branches) the `gh-pages` branch if you forked Minimal Mistakes. This branch contains the documentation and demo site for the theme and you probably don't want that showing up in your repo.
{: .notice--info}

## Customize Your Site

Open up `_config.yml` found in the root of the repo and edit anything under **Site Settings**. For a full explanation of every setting be sure to read the [**Configuration**]({{ base_path }}/docs/configuration/) section, but for now let's just change the site's title.

<figure>
  <img src="{{ base_path }}/images/mm-github-edit-config.gif" alt="editing _config.yml file">
  <figcaption>Edit text files without leaving GitHub.com</figcaption>
</figure>

Committing a change to `_config.yml` (or any file in your repository) will force GitHub Pages to rebuild your site with Jekyll. It should then be viewable a few seconds later at `https://USERNAME.github.io`.

---

Congratulations! You've successfully forked the theme and are up an running with GitHub Pages. Now you're ready to add content and customize the site further.
-->
