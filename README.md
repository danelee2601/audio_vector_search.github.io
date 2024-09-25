# Sound Effect Vector Search Demo

**Author:** Daesoo Lee  
**Company:** HANCE  

---

## Introduction

Welcome to the demo of our new method for Sound Effect Vector Search. This project aims to find the top **k** most similar sound effect files from the **Soundly database** based on a given audio file and/or text description. By providing both an audio reference and a text description, users can achieve the most accurate search results. However, the system is flexible and allows searches using either input individually.

## Method

Our method leverages advanced audio processing and natural language understanding techniques to map both sound files and textual descriptions into a shared vector space. This enables efficient similarity comparisons between different types of inputs. The core components of our method include:

- **Audio Feature Extraction:** Utilizing spectral analysis and temporal features to represent audio files numerically.
- **Text Embedding:** Employing state-of-the-art language models to encode text descriptions into vectors.
- **Similarity Computation:** Calculating cosine similarity between vectors to find the most similar sound effects.
- **Hybrid Matching:** Combining audio and text similarities when both inputs are provided to enhance search accuracy.

## Computational Efficiency

Efficiency is a critical aspect of our system, especially when dealing with large databases like Soundly. To ensure rapid search responses, we have implemented:

- **Vector Indexing:** Using efficient data structures like KD-Trees for quick nearest neighbor searches.
- **Dimensionality Reduction:** Applying techniques such as PCA to reduce computation without significant loss of accuracy.
- **Parallel Processing:** Leveraging multi-threading and GPU acceleration where applicable.

## Experimental Results

Below we present sample results from our system. Audio samples are provided to demonstrate the effectiveness of our search method.

### A. User Input: Reference Audio + Text Description

**Reference Audio:** [Audio Sample 1](#)  
**Text Description:** "Crashing ocean waves with distant seagulls"

| Rank | Similar Audio |
|------|---------------|
| 1    | [Audio Match 1](#) |
| 2    | [Audio Match 2](#) |
| 3    | [Audio Match 3](#) |
| 4    | [Audio Match 4](#) |
| 5    | [Audio Match 5](#) |

### B. User Input: Reference Audio

**Reference Audio:** [Audio Sample 2](#)

| Rank | Similar Audio |
|------|---------------|
| 1    | [Audio Match 1](#) |
| 2    | [Audio Match 2](#) |
| 3    | [Audio Match 3](#) |
| 4    | [Audio Match 4](#) |
| 5    | [Audio Match 5](#) |

### C. User Input: Text Description

**Text Description:** "Heavy thunderstorm with pouring rain"

| Rank | Similar Audio |
|------|---------------|
| 1    | [Audio Match 1](#) |
| 2    | [Audio Match 2](#) |
| 3    | [Audio Match 3](#) |
| 4    | [Audio Match 4](#) |
| 5    | [Audio Match 5](#) |

---

Feel free to explore the demo and experience the seamless integration of audio and text in searching for the perfect sound effect.