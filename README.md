# NLP Relation Extraction and Cognitive Mapping Demo

This repository contains a Jupyter Notebook demonstrating two Python applications:
1.  **Natural Language Processing (NLP) for Relation Extraction:** Using `spaCy`, this section processes sample sentences to identify named entities (PERSON, ORG) and extract "works for" relationships. These relationships are then visualized as a knowledge graph using `NetworkX` and `Matplotlib`.
2.  **Conceptual Cognitive Map Visualization:** Using `NetworkX`, this section constructs and visualizes a simple cognitive map, demonstrating how to represent causal or influential relationships, including conjunctive logic (AND-nodes).

## Purpose

This project showcases skills in:
*   Python programming
*   NLP with `spaCy` (tokenization, POS tagging, NER, dependency parsing)
*   Graph data structures and algorithms with `NetworkX`
*   Data visualization with `Matplotlib`
*   Structuring and presenting data-driven insights within a Jupyter Notebook environment.

## Files

*   `notebooks/your_actual_notebook_name.ipynb`: The main Jupyter Notebook containing all the code, explanations, and visualizations.
*   `requirements.txt`: A list of Python dependencies required to run the notebook.
*   `README.md`: This file.
*   `.gitignore`: Specifies intentionally untracked files that Git should ignore.

## Setup and Usage

1.  **Clone the repository (if you haven't already):**
    ```bash
    git clone https://github.com/RehamJamal13/nlp-cognitive-mapping-demo.git
    cd nlp-cognitive-mapping-demo
    ```

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Download spaCy model:**
    The notebook uses the `en_core_web_sm` model. If you don't have it, download it:
    ```bash
    python -m spacy download en_core_web_sm
    ```

5.  **Run Jupyter Notebook:**
    Start Jupyter Lab or Jupyter Notebook from the root directory:
    ```bash
    jupyter lab  # or jupyter notebook
    ```
    Then navigate to the `notebooks/` folder within the Jupyter interface and open `your_actual_notebook_name.ipynb`.

## Optional: Graphviz for Hierarchical Layout
The cognitive map visualization attempts to use Graphviz for a hierarchical layout (`dot` program). If Graphviz is not installed on your system, the plot will fall back to a spring layout. To install Graphviz:
*   **Linux (Ubuntu/Debian):** `sudo apt-get install graphviz`
*   **macOS (using Homebrew):** `brew install graphviz`
*   **Windows:** Download installers from the [Graphviz website](https://graphviz.org/download/) and ensure the `bin` directory is added to your system's PATH.
You may also need the `pydotplus` Python package (or `pydot`), which should be included in `requirements.txt` if you are using `nx.nx_pydot.graphviz_layout`.

## Author
Reham Jamal
