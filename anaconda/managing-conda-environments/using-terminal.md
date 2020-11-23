---
description: >-
  Alternatively, conda environments can managed using Terminal. In fact,
  everything on the GUI can be done with command lines. If you don't feel
  comfortable with this, please use Anaconda Navigator.
---

# Using Terminal

### Creating Environment

`conda create` creates a new environment in the _envs_ folder of your _anaconda3_ installation \(for example, on my Mac, the location is _/Applications/anaconda3/envs\)_. We can additionally specify the python version when creating the environment.

```
$ conda create -name project1 python=3.7
```

{% hint style="warning" %}
If you are on MacOS and using the zsh shell, you may have problems using conda. [Using Anaconda with zsh -&gt;](../zsh.md)
{% endhint %}

An environment is activated by calling `conda activate` with its name. Any scripts we run while the environment is activated will use the packages & versions installed within that environment. 

```
$ conda activate project1
```

### Managing Packages

We can easily add, upgrade, downgrade, and remove packages in the current environment with these commands. [More info -&gt;](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#updating-packages)

```bash
# list of installed packages in environment
$ conda list
# add package: use conda install [package name]
$ conda install -c conda-forge tensorflow
# update to latest version: use conda update [package name]
$ conda update tensorflow
# if downgrading version, specify version during install
$ conda install tensorflow=1.1
# remove package: use conda remove [package name]
$ conda remove tensorflow
```

### Deactivating Environment

To deactivate the conda environment, use `conda deactivate`. You can manage packages in deactivated environment by specifying the environment name with the commands. [More info -&gt;](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#updating-packages)

```text
$ conda deactivate
```

### Deleting Environment

If you wish to delete the environment completely, navigate to the _envs_ folder of your _anaconda3_ installation and remove the correct directory.

```bash
$ cd /Applications/anaconda3/envs
$ rm -r project1
```

