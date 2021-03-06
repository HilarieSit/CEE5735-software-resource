---
description: >-
  Anaconda Navigator is a graphical user interface (included in your
  installation of Anaconda) that lets you to access applications and manage
  conda environments without using Terminal.
---

# Using Navigator

### Documentation

{% embed url="https://docs.anaconda.com/anaconda/navigator/" %}

### Starting Navigator

Anaconda Navigator can be found on Launchpad \(Mac\) or start menu \(Windows\). The homepage displays applications, which can be installed and then launched. Default applications that are useful for this course are Jupyter Notebook \(an interactive computational environment that is great for displaying code & results\) and Spyder \(Python IDE\).

![](../../.gitbook/assets/screen-shot-2020-09-21-at-6.06.44-pm.png)

### Creating Environment

To create a conda environment, click on _Environments_ on the left navigation bar and then _create_ outlined in red. Name your environment and select the appropriate Python version.

![](../../.gitbook/assets/screen-shot-2020-09-21-at-7.21.31-pm.png)

The current environment is indicated with green. You can switch environments by clicking on tabs with the environment names.

### Managing Packages

We can filter the list of packages, shown on the right, to view the installed packages within the current environment.

![](../../.gitbook/assets/screen-shot-2020-09-27-at-12.13.31-am.png)

To add a package in the current environment, switch to _Uninstalled_ and then perform a search for the package name in Anaconda Cloud \(you do not need to sign in\). 

![](../../.gitbook/assets/screen-shot-2020-09-27-at-12.18.04-am.png)

Select the packages you want to add and select _Apply_ on the bottom right. To perform a package update, filter for _Updatable_ packages and mark the appropriate one for update.

![](../../.gitbook/assets/screen-shot-2020-09-27-at-12.14.13-am.png)

### Opening Terminal‌

You can open a terminal by clicking the right arrow and selecting _Open Terminal_. This automatically activates the environment and opens your terminal \(Mac\) or Anaconda prompt \(Windows\).

![](../../.gitbook/assets/screen-shot-2020-09-21-at-7.39.21-pm%20%281%29.png)

{% hint style="warning" %}
If you are on MacOS and using the zsh shell, you may get an error here. [Using Anaconda with zsh -&gt;](zsh.md)
{% endhint %}

