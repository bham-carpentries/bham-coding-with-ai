---
title: "Setup"
---

A practical introduction to using AI to support coding in research. This course will help researchers understand how to use AI to help them write code effectively and responsibly. This course is designed for researchers with little to no experience coding.  The course provides clear, hands-on guidance for using AI to write, debug, and understand code, while addressing key ethical, security, and reliability considerations in research contexts.


## Data Sets

Download the dataset we will work with by clicking here: [animals.csv](../episodes/data/animals.csv)

Save it to your desktop or another easily accessible location. 

::::::::::::::::::::::::::::::::::::: callout

## Where does the data come from?

The data we're working with comes from the [Portal Project](https://portal.weecology.org/), a long-term ecological study being conducted near Portal, Arizona. Since 1977, the site has been used to study interactions between rodents, ants and plants.

For this workshop, we use a CSV file that is a subset of the teaching-focused Portal dataset. This version has been simplified by removing some of the complexities of the full dataset, making it more suitable for computational training and learning exercises.

::::::::::::::::::::::::::::::::::::::::::::::::

## Software Setup

### AI Tool

You need to be able to access an AI Chat tool such as Microsoft CoPilot.

+ Navigate to <https://copilot.microsoft.com//> 
+ !IMPORTANT: Check that you are logged in using your work account
  (University of Birmingham email address) rather than your personal
  account.

### Python 

[Python](https://python.org) is widely used in research computing, and great for general-purpose programming tasks.  Installing all of its research packages individually can be a bit difficult, so we recommend [Conda-forge](https://conda-forge.org/download), an all-in-one installer.

Regardless of how you choose to install it, **please make sure you install a Python version >= 3.9** (e.g. 3.11 is fine, 3.6 is not).

We will teach Python using the [Jupyter Notebook](https://jupyter.org), a programming environment that runs in a web browser (Jupyter Notebook will be installed by Miniforge). For this to work you will need a reasonably up-to-date browser. The current versions of the Chrome, Safari and Firefox browsers are all [supported](https://jupyter-notebook.readthedocs.io/en/stable/notebook.html#browser-compatibility) (some older browsers, including Internet Explorer version 9 and below, are not).

#### Steps:

1. If you already have Python 3.9 or later installed and can run Jupyter Notebooks or Jupyter Lab, you can skip ahead to step 2.

::::::::::::::::::::::::::::::::::::::::::::::: tab

### Lab PC

  a. Open [AppsAnywhere](https://apps.bham.ac.uk) from the Windows Desktop.
  b. Login to your University Microsoft account when prompted.
  c. Allow the browser to open the AppsAnywhere browser.
  d. In the search bar, search for "miniforge", which should bring up "Miniforge Python 24.3.0-0 with All school addons".
  e. Select "Launch" next to Miniforge or on its description page.
  f. When ready, launch Miniforge by pressing the Launch icor or double-clicking.
  g. This brings up a file folder, where you should double-click on "Miniforge Prompt".

### Other

a. Follow Miniforge's [download and installation](https://conda-forge.org/download/) and instructions for your respective operating system. If you are using a Windows machine, make sure you mark the option to "Add Miniforge3 to my PATH environment variable".
b. If you are using Mac or Linux, open the 'Terminal'. If you are using Windows, open the 'Command Prompt' or 'Miniforge Prompt'.

::::::::::::::::::::::::::::::::::::::::::::::::::::::


2. Activate the base conda environment by typing and running the code below to activate your environment.

```terminal
conda activate
```

### Jupiter Lab and Other Dependencies


3. Install the necessary packages by running:
```terminal
pip install pandas matplotlib jupyterlab
```

4. Start Jupyter Lab by running: 
```terminal
jupyter lab
```

5. In a new Jupyter Notebook run the following code in a cell to check the necessary libraries can be loaded:
```python
import matplotlib as plt
import pandas as pd
```

