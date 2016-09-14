---
title: "First Time Use"
permalink: /docs/first-time-use/
excerpt: "Doing the first analysis with the uslfin package."
modified: 2016-09-14T18:02:00-01:00
---

{% include base_path %}

Running experiments with the package is very easy. There is even a top-level function that does a series of experiments. It only needs required inputs and parametrizations. Rest of it is quite automatic and convenient. In this example, we will cluster pricing errors using different K-Means parametrizations.

# Step 1 - Save input parameters Excel File

Just download the [input_parameters.xlsx]({{ base_path }}/files/input_parameters.xlsx) file from this github repository to a folder of your choice. But, remember your choice because we are going to use it.

# Step 2 - Run the code

Run the code given in the gist changing the `setwd` value.

{% gist 6df145c579806799122c492465c2ffde first_time_use_uslfin.r %}

# Step 3 - See the results

Your output should be something similar to the figure below.

<figure>
  <img src="{{ base_path }}/images/uslfin-first-use-example.png" alt="First Use Results">
</figure>

# What is next?

Congratulations, you have made this far! Now, you can meddle with the function, try different data sets and data mining methods. See other sections of this tutorial for further information.

You can see different parameter values of the `run_full_experiment` function by writing `?run_full_experiment` to the R console. The help file will appear with the detailed information about the function and its parameters.
{: .notice--info}

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
