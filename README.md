# Create Python Project Script

This script helps automate the creation of new Python projects on macOS. It sets up the basic structure of a Python project.

## Features

- Sets up a basic Python project structure.
- Creates virtual environments (optional, can be configured in the scrip).

## Usage

### 1. **Place the Script in a Directory in Your PATH**

To run the `create_py` script from anywhere on your system, you need to place it in a directory that’s in your `PATH`.

- You can move the `create_py` script to any directory that is already in your `PATH`, such as `/usr/local/bin/` or `$HOME/bin/`.

Alternatively, you can create a new directory for your custom scripts and add it to your `PATH`. For example:

1. Create a new directory for your scripts:   
   ```bash
   mkdir -p $HOME/create-python-project
   ```

2. Move the `create_py` script to that directory:
   ```bash
   mv /usr/local/bin/create_py $HOME/create-python-project/create_py
   ```

3. Update your `PATH` by adding the following line to your `~/.zshrc` (or `~/.bash_profile` if you use Bash):
   ```bash
   export PATH=$PATH:$HOME/create-python-project
   ```

4. After updating your `~/.zshrc` or `~/.bash_profile`, reload it:
   ```bash
   source ~/.zshrc  # for Zsh users
   source ~/.bash_profile  # for Bash users
   ```

### 2. **Run the Script**

Once the script is added to your `PATH`, open a terminal and run the following command to create a new Python project:

```bash
create_py
```

### 3. **Example Output:**

```bash
maxkoste:~ % create_py
Type the project name: cool_project
Venv created!
project activated
main.py created
Would you like to open the project? y/n
y
```
