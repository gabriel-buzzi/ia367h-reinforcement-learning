# IA367H - Introduction to Reinforcement Learning Course
## FEEC - Unicamp

Repository dedicated to IA367H course at FEEC-Unicamp on 2025S2

## Contributing
#### Clone the Repository

Use the following code to clone this repository.
```bash
git clone https://github.com/gabriel-buzzi/ia367h-reinforcement-learning.git
```

#### Install Pixi

[Pixi](https://pixi.sh/latest/) is a fast, modern, and reproducible package management tool for developers of all backgrounds.

To install [Pixi](https://pixi.sh/latest/) run the following.

For Linux & macOS run the following:
```bash
curl -fsSL https://pixi.sh/install.sh | sh
```

Once you have Pixi installed navigate to the project root folder and run `pixi install` to setup the project environment.

#### Install LaTeX

This project includes a set of `.tex` files for writting a paper. To render LaTeX files install the following

```bash
sudo apt install texlive
```

If the LaTeX project is more complex, you might need to install the full version of texlive with the following
```bash
sudo apt install texlive-full
```

In order to work with LaTeX on VSCode it is highly recommended to install **LaTeX Workshop** extension.

#### Ruff

[Ruff](https://docs.astral.sh/ruff/) is an extremely fast Python linter and code formatter, written in Rust. Ruff rules will be forced on code inside `ia367h-rl` folder. Ruff should be installed as a project dependency as you run any `pixi` command.

One can update Ruff configs within `pyproject.toml`.

In order to have a better experience with Ruff, it is recommended to install the **Ruff** VSCode extension and used its shortcuts while writting code.

#### Install pre-commit

Pre-commits are scripts called every time you commit something to the repository. In orther to be able to commit you code you should have pre-commit install, for that run the following:

```
pip install pre-commit
pre-commit install
```

The only pre-commit hook condigured by now is the Ruff pre-commit for code linting and formatting. This should enforce code inside `/ia367h-rl` to follow the Ruff rules defined at `pyproject.toml`. `.ipynb` files inside `/notebooks` are ignored by Ruff pre-commit hooks.

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

