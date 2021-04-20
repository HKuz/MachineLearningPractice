# Plants Project

## Data

This project uses data that indicate the presence of different plant species in various US states and Canadian provinces. It is located in the [UCI Machine Learning Repository Plants dataset folder](https://archive.ics.uci.edu/ml/datasets/Plants).

The original data are courtesy of USDA, NRCS. 2008. The [PLANTS Database](http://plants.usda.gov/), 31 December 2008). National Plant Data Center, Baton Rouge, LA 70874-4490 USA.

The `plants.data` and `plants.names` files appear to use the `ISO-8859-1` (aka `latin1`) encoding as determined with 73% confidence by the `chardet` package.

## Virtual Environment

The project depends on a variety of Python packages, all of which are listed in the `requirements.txt` file. To install the virtual environment locally, run the following command from your project folder:

```bash
# Unix/macOS
python3 -m pip install -r requirements.txt

# Windows
py -m pip install -r requirements.txt
```

Activate the environment with the following command, where `<DIR>` indicates the name of the virtual environment directory.

```bash
# Unix/macOS
source <DIR>/bin/activate

# Windows
<DIR>\Scripts\activate
```

To launch a Jupyter notebook (which is necessary to work in the analysis `.ipynb` files), first make sure your current virtual environment is activated, then run the `jupyter notebook` command. If the notebook can't find packages that are installed in the virtual environment, you may need to manually create a kernel. Close out of your current Jupyter session, again make sure the virtual environment is activated, then run:

```bash
ipython kernel install --user --name=<DIR>
```

Then re-launch your Jupyter session via the `jupyter notebook` command and open a `.ipynb` file. In the Kernel menu, select "Change Kernal", then find the newly created kernel in the list. It will have whatever name you specified in the `--name` field when you installed the kernel.
