Since you're using **Windows** and **Python is already installed**, the easiest way is:

### 1. Open Command Prompt

Press **Windows + R**, type:

```text
cmd
```

and press **Enter**.

### 2. Check Python

```bash
python --version
```

You should see something like:

```text
Python 3.13.14
```

### 3. Install Jupyter Notebook

Run:

```bash
python -m pip install notebook
```

Wait until the installation finishes.

### 4. Start Jupyter Notebook

Run:

```bash
jupyter notebook
```

Jupyter Notebook should open automatically in your browser.

### 5. Create your first notebook

In the Jupyter interface:

**New → Python 3 (ipykernel)**

Then you can start writing Python code.

### If `jupyter notebook` doesn't work

Try:

```bash
python -m notebook
```

**My recommendation for you:** Since you're learning **Python and Data Analytics**, install Jupyter Notebook using `pip` as above. You can then use it with **Pandas, NumPy, Matplotlib, and Scikit-learn**.
