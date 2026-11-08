## Installing Qiskit Using a Python Virtual Environment

This section describes how to install Qiskit in an isolated Python environment on macOS.

### 1. Create a Virtual Environment

Create a virtual environment named `qiskit_env` in the user's home directory:

```bash
python3 -m venv ~/qiskit_env
```

**Explanation:**
- `python3`: Runs the Python 3 interpreter.
- `-m venv`: Executes Python's built-in virtual environment module.
- `~/qiskit_env`: Creates the environment in the user's home directory.

### 2. Activate the Virtual Environment

```bash
source ~/qiskit_env/bin/activate
```

After activation, the terminal prompt displays `(qiskit_env)`:

```bash
(qiskit_env) BADWLRZ-CM06214:qiskit di97qid$
```

This indicates that commands using `python` and `pip` will use the virtual environment rather than the system-wide Python installation.

### 3. Upgrade pip

Upgrade pip to its latest available version:

```bash
python -m pip install --upgrade pip
```

**Explanation:**
- `python -m pip`: Executes pip through the active Python interpreter.
- `install --upgrade pip`: Installs or upgrades pip to the latest available version.

The installation was successful:

```text
Successfully installed pip-26.0.1
```

### 4. Install Qiskit

Install Qiskit using pip:

```bash
python -m pip install qiskit
```

### 5. Verify the Installation

Check whether Qiskit was installed successfully:

```bash
python -c "import qiskit; print(qiskit.__version__)"
```

If the installation is successful, the command displays the installed Qiskit version.

### 6. Deactivate the Environment

When finished, deactivate the virtual environment:

```bash
deactivate
```

To use Qiskit again, reactivate the environment:

```bash
source ~/qiskit_env/bin/activate
```

**Note:** The virtual environment keeps Qiskit and its Python dependencies isolated from the system-wide Python installation. Activate it whenever you want to work with this Qiskit environment.
