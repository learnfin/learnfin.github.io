---
title: "First Time Use"
permalink: /docs/first-time-use/
excerpt: "Doing the first analysis with the learnfin package."
modified: 2016-09-14T18:02:00-01:00
---

{% include base_path %}

Running experiments with the package is very easy. There is even a top-level function that does a series of experiments. It only needs required inputs and parametrizations. Rest of it is quite automatic and convenient. In this example, we will cluster pricing errors using different K-Means parametrizations.

# Step 1 - Save input parameters Excel File

Just download the [input_parameters.xlsx]({{ base_path }}/files/input_parameters.xlsx) file from this github repository to a folder of your choice. But, remember your choice because we are going to use it.

# Step 2 - Run the code

Run the code given in the gist changing the `setwd` value.

{% gist 6df145c579806799122c492465c2ffde first_time_use_learnfin.r %}

# Step 3 - See the results

Your output should be something similar to the figure below.

<figure>
  <img src="{{ base_path }}/images/learnfin-first-use-example.png" alt="First Use Results">
</figure>

# What is next?

Congratulations, you have made this far! Now, you can meddle with the function, try different data sets and data mining methods. See other sections of this tutorial for further information.

You can see different parameter values of the `run_full_experiment` function by writing `?run_full_experiment` to the R console. The help file will appear with the detailed information about the function and its parameters.
{: .notice--info}
