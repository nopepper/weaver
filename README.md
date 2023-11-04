# Weaver: Document Linking Made Easy

<p align="center">
  <img src="icon.png" width="300" />
</p>

<p align="center">
<i>Named after the bird known for its intricately woven nests, Weaver connects documents by identifying key entities and linking them to relevant documents in the set.</i>
</p>

# Overview

Weaver is a machine learning tool designed to generate Wikipedia-style connections between a set of text documents. 

## Features

1. **Document Encoding:** Weaver uses advanced sentence transformers to generate vector representations of each document, capturing the semantic meaning in a compact form.

2. **Entity Identification & Linking:** Leveraging a fine-tuned BERT-based classifier, Weaver identifies tokens that are part of a link and generates a "link embedding". This embedding has a high cosine similarity with the document vector it links to, effectively creating a neural pointer to the relevant document.

3. **Easy Integration:** Weaver is designed to be easily integrated into your existing text processing pipeline. It can handle a wide range of document types and sizes.

# Getting Started

TODO

## Docker

Build:
docker build -t weaver .

Run:
docker run -p 8000:80 -v .:/app --gpus all weaver