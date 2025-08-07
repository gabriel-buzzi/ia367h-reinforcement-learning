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

## Project Organization

```
├── LICENSE            <- Open-source license if one is chosen
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default mkdocs project; see www.mkdocs.org for details
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
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
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

