# Persian Data Retrieval System

This project implements a Persian text retrieval system that leverages positional indexing and TF-IDF weighting to enable efficient and accurate document retrieval. The system builds an index that tracks the positions of words within documents, computes term weights, and supports advanced query processing using phrase and proximity searches.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [License](#license)

## Overview

The Persian Data Retrieval System is designed to:
- Index a collection of Persian news articles.
- Build a positional index that records word positions in each document.
- Calculate TF-IDF weights for each term in the collection.
- Create a champions list for each term to improve query performance.
- Process user queries (including phrase queries) to return the most relevant documents.

This project is intended as part of a larger information retrieval system and serves as a foundation for more advanced retrieval techniques and evaluation metrics.

## Features

- **Positional Indexing:** Tracks the positions of each word in the documents, enabling support for phrase and proximity queries.
- **TF-IDF Weighting:** Computes term frequency and inverse document frequency to determine the importance of each term in a document.
- **Champions List:** Generates a ranked list of documents (champions) for each term, reducing the number of documents to be scanned during query processing.
- **Document Norms:** Calculates normalized weights for documents to facilitate cosine similarity-based ranking.
- **Query Processing:** Supports basic query processing that utilizes the positional index for retrieving matching documents.

## Installation

1. **Clone the Repository:**

   ```bash
   git clone git@github.com:your-username/persian-data-retrieval-system.git
   cd persian-data-retrieval-system
2. **Set Up Virtual Environment:**

   It is recommended to use a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt

**Usage**
**1. Building the Index and Computing Weights:**

Run the main script or open the Jupyter Notebook (main.ipynb) to build the positional index and calculate term frequencies and TF-IDF scores:

  ```bash
  jupyter notebook main.ipynb
  ```
The notebook will:

-Load the dataset.
-Build the positional index and compute term frequencies.
-Calculate IDF and TF-IDF scores.
-Save the positional index and TF-IDF scores as JSON files.
-Provide an example query to demonstrate the retrieval process.

**2. Querying:**

Modify the query string in the notebook to test different search phrases. The system will return a list of document IDs that match the query based on their positional information and computed weights.


Reasoned for a second
Below is a complete README.md file in Markdown format, including a link to the dataset:

markdown
Copy
Edit
# Persian Data Retrieval System

This project implements a Persian text retrieval system that leverages positional indexing and TF-IDF weighting to enable efficient and accurate document retrieval. The system builds an index that tracks the positions of words within documents, computes term weights, and supports advanced query processing using phrase and proximity searches.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Future Work](#future-work)
- [License](#license)

## Overview

The Persian Data Retrieval System is designed to:
- Index a collection of Persian news articles.
- Build a positional index that records word positions in each document.
- Calculate TF-IDF weights for each term in the collection.
- Create a champions list for each term to improve query performance.
- Process user queries (including phrase queries) to return the most relevant documents.

This project is intended as part of a larger information retrieval system and serves as a foundation for more advanced retrieval techniques and evaluation metrics.

## Features

- **Positional Indexing:** Tracks the positions of each word in the documents, enabling support for phrase and proximity queries.
- **TF-IDF Weighting:** Computes term frequency and inverse document frequency to determine the importance of each term in a document.
- **Champions List:** Generates a ranked list of documents (champions) for each term, reducing the number of documents to be scanned during query processing.
- **Document Norms:** Calculates normalized weights for documents to facilitate cosine similarity-based ranking.
- **Query Processing:** Supports basic query processing that utilizes the positional index for retrieving matching documents.

## Installation

1. **Clone the Repository:**

   ```bash
   git clone git@github.com:your-username/persian-data-retrieval-system.git
   cd persian-data-retrieval-system
Set Up Virtual Environment:

It is recommended to use a virtual environment:

  ```bash
  python3 -m venv venv
  source venv/bin/activate
  ```
Install Dependencies:

Install the required packages:

  ```bash
  pip install -r requirements.txt
  ```
## Usage
Building the Index and Computing Weights:

Run the main script or open the Jupyter Notebook (main.ipynb) to build the positional index and calculate term frequencies and TF-IDF scores:

  ```bash
  jupyter notebook main.ipynb
  ```
The notebook will:

Load the dataset.
Build the positional index and compute term frequencies.
Calculate IDF and TF-IDF scores.
Save the positional index and TF-IDF scores as JSON files.
Provide an example query to demonstrate the retrieval process.
Querying:

Modify the query string in the notebook to test different search phrases. The system will return a list of document IDs that match the query based on their positional information and computed weights.

## Dataset
The dataset used in this project can be downloaded from the following link:
[IR_data_news_12k.json]([https://example.com](https://drive.google.com/file/d/1x-ypTPZ0R_T83YfCw-p55MaQtpCvkrsb/view))

## Project Structure
  ```bash
  persian-data-retrieval-system/
│
├── data/                      # Contains the dataset (this directory is ignored by Git)
├── main.ipynb                 # Jupyter Notebook with the implementation and examples
├── requirements.txt           # List of project dependencies
├── venv/                      # Virtual environment (optional)
└── README.md                  # Project documentation
```

## License
```yaml

---

Simply copy this content into a file named `README.md` in your repository's root directory. Adjust the repository URL, dataset path, and any additional details as needed for your specific implementation.
