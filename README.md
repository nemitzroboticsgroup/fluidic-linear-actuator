# JupyterLab Installation Guide

This guide will help you install JupyterLab, set up a virtual environment, and import an existing notebook file named `analytical-model.ipynb`.

## Table of Contents
- [Why Use a Virtual Environment](#why-use-a-virtual-environment)
- [Step 1: Install Python](#step-1-install-python)
- [Step 2: Set Up a Virtual Environment](#step-2-set-up-a-virtual-environment)
- [Step 3: Install JupyterLab](#step-3-install-jupyterlab)
- [Step 4: Import a Notebook File](#step-4-import-a-notebook-file)
- [Additional Resources](#additional-resources)

---

## Why Use a Virtual Environment

Virtual environments allow you to create isolated environments for different Python projects. Each environment can have its own dependencies, which prevents package conflicts and ensures your projects remain organized. This is especially helpful when managing multiple projects that require different versions of libraries or Python itself.

---

## Step 1: Install Python

Before setting up JupyterLab, make sure you have Python installed. You can check if Python is installed by running the following command in your terminal:

```bash
python3 --version
```

If Python is not installed, you can download it [here](https://www.python.org/downloads/) or use a package manager like **Homebrew**:

```bash
brew install python
```

---

## Step 2: Set Up a Virtual Environment

### Install `virtualenv`

To create a virtual environment, we’ll use Python's `virtualenv` tool. If you don’t have it installed, run the following command:

```bash
pip3 install virtualenv
```

### Create a Virtual Environment

Once `virtualenv` is installed, create a new environment:

```bash
python3 -m venv myenv
```

Here, `myenv` is the name of your environment. You can name it anything you like.

### Activate the Virtual Environment

Activate the environment to start working within it:

- On **macOS/Linux**:

  ```bash
  source myenv/bin/activate
  ```

- On **Windows**:

  ```bash
  myenv\Scripts\activate
  ```

Once activated, you should see `(myenv)` at the beginning of your terminal prompt. This means you're inside the virtual environment.

### Deactivating the Virtual Environment

To deactivate the environment when you're done:

```bash
deactivate
```

---

## Step 3: Install JupyterLab

With the virtual environment activated, install JupyterLab using `pip`:

```bash
pip install jupyterlab
```

Once the installation completes, you can launch JupyterLab by running:

```bash
jupyter lab
```

This will open JupyterLab in your browser, where you can create, edit, and run notebooks.

---

## Step 4: Import a Notebook File

If you have a notebook file like `analytical-model.ipynb` that you want to open in JupyterLab, follow these steps:

1. Make sure the `analytical-model.ipynb` file is located in the same directory where you started JupyterLab or navigate to the correct directory within JupyterLab's file browser.

2. Launch JupyterLab:

   ```bash
   jupyter lab
   ```

3. In the JupyterLab interface, you’ll see a file browser on the left. Find and click on `analytical-model.ipynb` to open it.

4. Once opened, you can edit, run, and analyze the notebook.

---

## Additional Resources

- [JupyterLab Documentation](https://jupyterlab.readthedocs.io/)
- [Python Virtual Environment Guide](https://docs.python.org/3/tutorial/venv.html)
- [Pip Package Manager](https://pip.pypa.io/en/stable/)
