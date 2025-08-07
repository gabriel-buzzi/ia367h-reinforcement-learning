# IA367H - Introduction to Reinforcement Learning Course
## FEEC - Unicamp

Repository dedicated to IA367H course at FEEC-Unicamp on 2025S2

## Contributing

It is **strongly recommend** using **Linux** when contributing to this project.
If you're using **Windows**, you might install the **Windows Subsystem for Linux (WSL)** before proceeding.

> ⚠️ The instructions below are intended for **Linux environments**.
> If you want to contribute from a native Windows setup (not using WSL), please refer to the official documentation for each tool to perform the appropriate setup.

---

### Setting Up WSL on Windows (Quick Guide)

1. **Open PowerShell as Administrator**
   Right-click the Start menu and choose **Windows Terminal (Admin)** or **PowerShell (Admin)**.

2. **Install WSL and Ubuntu**
   Run the following command:

   ```powershell
   wsl --install
   ```

   This installs WSL with Ubuntu as the default distribution.
   Restart your computer if prompted.

3. **Initial Ubuntu Setup**
   After reboot, a terminal window will open.
   Follow the instructions to create your Linux username and password.

4. **Update Ubuntu Packages**
   Inside the Ubuntu terminal, run:

   ```bash
   sudo apt update && sudo apt upgrade -y
   ```

✅ You're now ready to proceed with the Linux-based setup steps below.

---

### Clone the Repository

Use the following command to clone the repository:

```bash
git clone https://github.com/gabriel-buzzi/ia367h-reinforcement-learning.git
cd ia367h-reinforcement-learning
```

---

### Install Pixi

[Pixi](https://pixi.sh/latest/) is a modern and fast package manager for reproducible development environments.

To install Pixi on Linux or macOS:

```bash
curl -fsSL https://pixi.sh/install.sh | sh
```

Then, in the project root directory, run:

```bash
pixi install
```

This sets up all project dependencies defined in `pyproject.toml`.

---

### Install LaTeX

This project includes LaTeX files used to write a paper. To compile LaTeX documents, install:

```bash
sudo apt install texlive
```

If you encounter missing packages or prefer a more complete setup, install the full distribution:

```bash
sudo apt install texlive-full
```

> 💡 **Tip:** For a better LaTeX editing experience in VSCode, install the **LaTeX Workshop** extension.

---

### Ruff

[Ruff](https://docs.astral.sh/ruff/) is a fast Python linter and formatter written in Rust.
It is configured to enforce code style in the `ia367h-rl/` directory.

Ruff is included as a dependency in the Pixi environment. Configuration is managed in the `pyproject.toml` file.

> 💡 **VSCode users:** Install the **Ruff** extension to get inline feedback and use linting/formatting shortcuts while writing code.

---

### Pre-commit Hooks

This project uses [pre-commit](https://pre-commit.com/) to run automatic checks before each commit.

To install and enable it, run:

```bash
pip install pre-commit
pre-commit install
```

Currently, the only configured hook is **Ruff**, which checks and formats code inside `ia367h-rl/` according to the rules in `pyproject.toml`.

> 📝 **Note:** `.ipynb` files inside the `notebooks/` folder are excluded from pre-commit checks.

## Project Organization

```
├── README.md          <- The top-level README for developers using this project.
├── data               <- Store your data files inside this folder (all files here will be ignored by git).
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── pyproject.toml     <- Project configuration file with package metadata for 
│                         ia367h-rl and configuration for tools like black
│
├── references         <- Reference research papers and any other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   ├── paper          <- LaTeX files for final project paper
│   └── figures        <- Generated graphics and figures to be used in reporting
│
└── ia367h-rl   <- Source code for use in this project.
    │
    ├── __init__.py             <- Makes ia367h-rl a Python module
    │
    └── main.py                 <- Project main
```

--------

