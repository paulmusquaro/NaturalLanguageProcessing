# NaturalLanguageProcessing


###### NLP-Based Text Summarization with NLTK and SpaCy

This project demonstrates how to create a summary of a given text using natural language processing (NLP) libraries: **NLTK** and **SpaCy**. By processing the provided text, the project extracts the most important information using techniques such as tokenization, stop word removal, word frequency analysis, and sentence scoring. The main goal is to identify key sentences that best represent the original content.

---

## Features
- **Text Preprocessing**: Includes tokenization, stop word removal, and optional lemmatization or stemming.
- **Word Frequency Analysis**: Counts the occurrences of significant words in the text to determine importance.
- **Sentence Scoring**: Ranks sentences based on the significance of the words they contain.
- **Summary Generation**: Extracts the most meaningful sentences to form a concise summary.

---

## Key Technologies
- **NLTK (Natural Language Toolkit)**: For tokenization, stop word removal, and sentence segmentation.
- **SpaCy**: For advanced NLP tasks and processing, such as loading language models and lemmatization.
- **Python Libraries**:
  - `collections.defaultdict`: For efficient frequency counting and sentence scoring.
  - `heapq.nlargest`: For selecting the highest-scored sentences.

---

## Conda (Setup and Environment)

To make the project reproducible and ensure smooth package management, this project uses Conda as a package and environment manager. Below are the steps to set up the environment:


1. **Install Conda**:
If you haven't installed Conda yet, you can download it from the official [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html) websites. Anaconda is a larger distribution with more pre-installed packages, while Miniconda is a smaller, minimal version. Choose whichever suits your needs.

2. **Create a new environment:** Open your terminal and run the following command to create a new Conda environment with Python 3.7:

    ```bash
    conda create --name new_conda_env python=3.7
    ```

3. **Activate the environment:** Once the environment is created, activate it by running:

    ```bash
    conda activate new_conda_env
    ```

4. **Install required packages (Jupyter, SpaCy and NLTK)**

    ```bash
    conda install jupyter spacy nltk
    ```

5. **Run Jupyter Notebook**

    ```bash
    jupyter notebook
    ```

---

## Workflow
1. **Load and Prepare Text**:
   - Input the text to be summarized.
   - Perform preprocessing (remove special characters, tokenize text, and filter stop words).

2. **Frequency Analysis**:
   - Calculate word frequencies in the text.
   - Use these frequencies to determine the weight of each sentence.

3. **Generate Summary**:
   - Rank sentences based on their scores.
   - Select the top-ranked sentences to create the final summary.

---

## Example Summary Output
**Input Text**: A detailed description of the Space Shuttle **Discovery (OV-103)**, its achievements, historical significance, and engineering innovations.

**Generated Summary**:
> According to Wayne Hale, a flight director from Johnson Space Center, the Space Shuttle orbiter represents a “huge technological leap from expendable rockets and capsules to a reusable, winged, hypersonic, cargo-carrying spacecraft.” Although her base structure followed a conventional aircraft design, she used advanced materials that both minimized her weight for cargo-carrying purposes and featured low thermal expansion ratios, which provided a stable base for her Thermal Protection System (TPS) materials. Under Criterion A, Discovery is significant as the oldest of the three extant orbiter vehicles constructed for the Space Shuttle Program (SSP), the longest-running American space program to date; she was the third of five orbiters built by NASA. The Orbiter Discovery, OV-103, is considered eligible for listing in the National Register of Historic Places (NRHP) in the context of the U.S. Space Shuttle Program (1969-2011) under Criterion A in the areas of Space Exploration and Transportation and under Criterion C in the area of Engineering. In addition, Discovery was vital to the construction of the International Space Station (ISS); she flew thirteen of the thirty-seven total missions flown to the station by a U.S. Space Shuttle. Including her maiden voyage (launched August 30, 1984), Discovery flew to space thirty-nine times, more than any of the other four orbiters; she was also the first orbiter to fly twenty missions. Discovery was the first shuttle to fly with the redesigned SRBs, a result of the Challenger accident, and the first shuttle to fly with the Phase II and Block I SSME.

---

## How to Run
1. Clone the repository or copy the provided Python script.
2. Modify the `text` variable with the desired input text.
3. Run the script to generate the summary.

---

## Future Improvements
- Implement support for multilingual text summaries using SpaCy's multilingual models.
- Introduce extractive and abstractive summarization techniques.
- Add visualization tools to display word frequencies and sentence scores.

---

## License
This project is open-source and available under the [MIT License](LICENSE).