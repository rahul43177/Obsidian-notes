[[Basic Setup for FastAPI]]
A virtual environment in Python is an isolated environment that allows you to manage dependencies for different projects separately. This is particularly useful when you have multiple projects that require different versions of the same package or library. By using virtual environments, you can avoid conflicts between dependencies and maintain a clean global Python environment.

### Creating a Virtual Environment on macOS and Windows

#### Prerequisites

Before creating a virtual environment, ensure you have Python installed on your system. You can check this by running:

```bash
python --version
```

If you have multiple versions of Python installed, you might need to use `python3` instead of `python`.

#### Using `venv` Module

The `venv` module is included in Python 3.3 and later. It is the recommended way to create virtual environments.

##### macOS

1. **Open Terminal**.

2. **Navigate to your project directory**:

   ```bash
   cd /path/to/your/project
   ```

3. **Create a virtual environment**:

   ```bash
   python3 -m venv myenv
   ```

   Replace `myenv` with the name you want to give to your virtual environment.

4. **Activate the virtual environment**:

   ```bash
   source myenv/bin/activate
   ```

5. **Deactivate the virtual environment** when you're done:

   ```bash
   deactivate
   ```

##### Windows

1. **Open Command Prompt**.

2. **Navigate to your project directory**:

   ```cmd
   cd \path\to\your\project
   ```

3. **Create a virtual environment**:

   ```cmd
   python -m venv myenv
   ```

   Replace `myenv` with the name you want to give to your virtual environment.

4. **Activate the virtual environment**:

   ```cmd
   myenv\Scripts\activate
   ```

5. **Deactivate the virtual environment** when you're done:

   ```cmd
   deactivate
   ```

### Using `virtualenv` (Alternative)

`virtualenv` is a third-party tool that can be used to create virtual environments. It is useful if you are using an older version of Python that does not include the `venv` module.

1. **Install `virtualenv`**:

   ```bash
   pip install virtualenv
   ```

2. **Create a virtual environment**:

   ```bash
   virtualenv myenv
   ```

3. **Activate and deactivate** the virtual environment using the same commands as above for macOS and Windows.

By using virtual environments, you can manage dependencies for different projects independently, ensuring that each project has access to the specific packages and versions it requires.
