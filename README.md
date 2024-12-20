<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a id="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![Unlicense License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Radiology Dataset Summarization with LangChain and HuggingFace</h3>

  <p align="center">
    An asynchronous pipeline for summarizing radiology text data using advanced NLP tools.
    <br />
    <a href="#about-the-project"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="#usage">Usage Examples</a>
    ·
    <a href="#roadmap">Roadmap</a>
    ·
    <a href="#contact">Contact</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#features">Features</a></li>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

This project provides an asynchronous pipeline for summarizing text data from a radiology dataset using HuggingFace's Transformers, LangChain tools, and Google Colab as the execution environment. The system incorporates summarization and reasoning models to process the dataset efficiently.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Features
- **Dataset Loading**: Loads and shuffles the `Ka4on/radiology` dataset.
- **Summarization Model**: Uses HuggingFace's `facebook/bart-large-cnn` model for text summarization.
- **Reasoning Model**: Employs the `EleutherAI/gpt-neo-1.3B` model for reasoning tasks.
- **LangChain Agent**: Initializes a LangChain agent to manage the summarization tool.
- **Asynchronous Processing**: Utilizes `asyncio` for parallel processing of dataset entries.
- **GPU Support**: Automatically detects and utilizes GPU if available for faster inference.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

* [![HuggingFace][huggingface-shield]][huggingface-url]
* [![LangChain][langchain-shield]][langchain-url]
* [![Google Colab][colab-shield]][colab-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

This is an example of how to set up and run the pipeline locally or on Google Colab.

### Prerequisites

Ensure the following libraries are installed:

```bash
pip install langchain==0.3.12 rouge_score langchain-community transformers torch sentence-transformers datasets evaluate
```

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/github_username/radiology_summary.git
   ```
2. Install required dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Configure runtime for GPU if using Google Colab.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Run the `main` script to process the radiology dataset.

```bash
python main.py
```

Example Outputs:
- Summarized Report
- Reasoning-based Insights

_For detailed examples, please refer to the [Documentation](#)._ 

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [x] Add GPU support
- [x] Include reasoning model
- [ ] Enhance summarization with fine-tuned models
- [ ] Add error correction mechanisms

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Your Name - [@your_twitter](https://twitter.com/your_username) - email@example.com

Project Link: [https://github.com/github_username/radiology_summary](https://github.com/github_username/radiology_summary)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
[huggingface-shield]: https://img.shields.io/badge/HuggingFace-yellow?style=for-the-badge&logo=huggingface
[huggingface-url]: https://huggingface.co
[langchain-shield]: https://img.shields.io/badge/LangChain-blue?style=for-the-badge
[langchain-url]: https://langchain.com
[colab-shield]: https://img.shields.io/badge/Google%20Colab-orange?style=for-the-badge&logo=googlecolab
[colab-url]: https://colab.research.google.com

