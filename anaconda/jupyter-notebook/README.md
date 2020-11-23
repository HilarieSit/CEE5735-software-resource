---
description: >-
  Jupyter notebook is a web application for developing, documenting, & sharing
  code. It's become pretty popular among data scientists for visualizing &
  analyzing datasets, but there's some limitations.
---

# Jupyter Notebook

### Starting Jupyter Notebook

Jupyter Notebook is one of the default applications on the Navigator home tab. Another way is to open it with Terminal; make sure that you are in the correct directory and then use the following command:

```bash
$ jupyter notebook
```

The Jupyter dashboard should open on your default web browser:

![](../../.gitbook/assets/screen-shot-2020-09-29-at-12.19.39-am.png)

Navigate into your desired directory and then select _Python 3_ under _New_ to create a Python 3 Notework. This will open up an empty notebook, which you can then name by clicking on _Untitled_. To open a pre-existing notebook, simply click on the .iypnb file and make sure that the kernel is connected.

![](../../.gitbook/assets/screen-shot-2020-09-29-at-12.27.09-am.png)

### Understanding Cells

Within a coding **cell**, you can write snippets of code. When you run a cell, the code is sent to a **kernel** that executes it. Variables can be called/used from previously ran cells.

![](../../.gitbook/assets/screen-shot-2020-09-28-at-11.27.19-pm%20%281%29.png)

To run a cell, you can either click on the _Run_ button or use Ctrl/Command - Enter. A running cell is indicated by an asterisk. Once the cell has finished running, the asterisk is replaced by a number that tells you the number of cells that you have ran up to that point. 

![](../../.gitbook/assets/screen-shot-2020-09-29-at-11.40.07-am.png)

{% hint style="danger" %}
Be careful about the order. Cells can be executed out of order or moved around and variables can be overwritten.
{% endhint %}

The Markdown cells allow you to add documentation to your code. Headings can be created using hashtags: \# Heading 1, \#\# Heading 2.

![](../../.gitbook/assets/screen-shot-2020-09-28-at-11.38.43-pm.png)

### Stopping Jupyter Notebook

To shutdown a running notebook, select the box and click _Shutdown._

![](../../.gitbook/assets/screen-shot-2020-09-29-at-11.23.48-am.png)

To exit Jupyter Notebook, click _Quit_ on the upper left corner or use Ctrl/Command - C in the Terminal.

