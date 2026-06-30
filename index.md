---
layout: default
title: CKGE-FMOC Tutorial
---

# CKGE-FMOC: Continual Knowledge Graph Embedding: Foundations, Methods, and Open Challenges

### A Tutorial at the **25th International Semantic Web Conference (ISWC 2026)**
**Date:** October 25 - 29, 2026  
**Venue:** The Nicolaus Hotel, Bari, Italy  

---

## Abstract
Knowledge Graph Embeddings (KGEs) provide fixed-length vector representations of entities and relations within a Knowledge Graph (KG), enabling a wide variety of downstream tasks over KGs. However, real-world KGs are dynamic, and continuously evolve with the addition of new entities, relations, and facts. Updating embeddings to reflect this growth without constantly retraining models from scratch, which is costly, presents a significant challenge. While generic continual learning approaches, such as fine-tuning, can be applied, they often fail to leverage the unique properties of KGs.

Since late 2023, a new research direction, Continual Knowledge Graph Embedding (CKGE), has emerged to address this limitation. There is a growing interest in the field, with nearly twenty specialized methods proposed in recent years. This tutorial aims to first introduce the fundamentals and motivation behind KGEs, and then provide a comprehensive overview of CKGE. We present a structured categorization of state-of-the-art approaches, highlighting their underlying principles and differences, as well as the evaluation protocols and metrics specific to continual settings. In addition, we examine the problem of catastrophic forgetting, analyzing its causes in evolving KGs and its impact on model performance. The tutorial concludes by discussing open challenges and promising directions for future research in CKGE.

---

## Presenters

<div style="display: flex; flex-direction: column; gap: 30px; margin-top: 20px;">
  
  <div style="display: flex; align-items: center; gap: 20px; flex-wrap: wrap;">
    <img src="images/presenter1.jfif" alt="Presenter 1 Name" style="width: 150px; height: 150px; border-radius: 50%; object-fit: cover; flex-shrink: 0; border: 2px solid #ddd;">
    <div style="flex: 1; min-width: 250px;">
      <h3 style="margin-top: 0;">Presenter One Name</h3>
      <p style="margin: 5px 0;"><em>Affiliation / University / Company</em></p>
      <p style="margin: 0;">Provide a short biography for the first presenter here. Mention their research interests, notable publications in KGE or Continual Learning, and any previous tutorial experience.</p>
    </div>
  </div>

  <div style="display: flex; align-items: center; gap: 20px; flex-wrap: wrap;">
    <img src="images/presenter2.jfif" alt="Presenter 2 Name" style="width: 150px; height: 150px; border-radius: 50%; object-fit: cover; flex-shrink: 0; border: 2px solid #ddd;">
    <div style="flex: 1; min-width: 250px;">
      <h3 style="margin-top: 0;">Presenter Two Name</h3>
      <p style="margin: 5px 0;"><em>Affiliation / University / Company</em></p>
      <p style="margin: 0;">Provide a short biography for the second presenter here. Highlight their specific contributions to the foundations, methods, or open challenges discussed in this session.</p>
    </div>
  </div>

</div>

---

## Schedule

<table style="width: 100%; border-collapse: collapse; text-align: left;">
  <thead>
    <tr style="background-color: #f6f8fa; border-bottom: 2px solid #d0d7de;">
      <th style="padding: 12px; width: 25%;">Time Slot</th>
      <th style="padding: 12px; width: 20%;">Time</th>
      <th style="padding: 12px; width: 55%;">Program & Materials</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid #d0d7de;">
      <td rowspan="2" style="padding: 12px; font-weight: bold; vertical-align: top; background-color: #fafafa;">Slot 1: Foundations</td>
      <td style="padding: 12px; vertical-align: top;">09:00 - 09:45</td>
      <td style="padding: 12px; vertical-align: top;">
        <strong>Introduction to KGE & The Streaming Challenge</strong><br>
        A brief recap of traditional Knowledge Graph Embeddings and why static models fail in dynamic environments. 
        <br><a href="slides/part1_foundations.pdf" target="_blank" style="font-weight: bold; text-decoration: underline;">[Download PDF Slides]</a>
      </td>
    </tr>
    <tr style="border-bottom: 1px solid #d0d7de;">
      <td style="padding: 12px; vertical-align: top;">09:45 - 10:30</td>
      <td style="padding: 12px; vertical-align: top;">
        <strong>Catastrophic Forgetting in KGs</strong><br>
        Formalizing the stability-plasticity dilemma when learning continuously over evolving facts.
        <br><a href="slides/part2_forgetting.pdf" target="_blank" style="font-weight: bold; text-decoration: underline;">[Download PDF Slides]</a>
      </td>
    </tr>
    <tr style="border-bottom: 1px solid #d0d7de;">
      <td rowspan="2" style="padding: 12px; font-weight: bold; vertical-align: top; background-color: #fafafa;">Slot 2: Methods</td>
      <td style="padding: 12px; vertical-align: top;">11:00 - 11:45</td>
      <td style="padding: 12px; vertical-align: top;">
        <strong>Current Continual Learning Paradigms</strong><br>
        Reviewing regularization-based, replay-based, and architecture-based methods adapted for graph structures.
        <br><a href="slides/part3_methods.pdf" target="_blank" style="font-weight: bold; text-decoration: underline;">[Download PDF Slides]</a>
      </td>
    </tr>
    <tr style="border-bottom: 1px solid #d0d7de;">
      <td style="padding: 12px; vertical-align: top;">11:45 - 12:30</td>
      <td style="padding: 12px; vertical-align: top;">
        <strong>Evaluation Frameworks & Benchmarks</strong><br>
        How to rigorously track training pipelines, backward transfer, and forward transfer performance.
        <br><a href="slides/part4_evaluation.pdf" target="_blank" style="font-weight: bold; text-decoration: underline;">[Download PDF Slides]</a>
      </td>
    </tr>
    <tr style="border-bottom: 1px solid #d0d7de;">
      <td rowspan="1" style="padding: 12px; font-weight: bold; vertical-align: top; background-color: #fafafa;">Slot 3: Open Challenges</td>
      <td style="padding: 12px; vertical-align: top;">14:00 - 15:30</td>
      <td style="padding: 12px; vertical-align: top;">
        <strong>The Road Ahead & Interactive Discussion</strong><br>
        Exploring unaddressed gaps like zero-shot entity alignment, scalability issues, and industry deployment hurdles followed by an open Q&A session.
        <br><a href="slides/part5_challenges.pdf" target="_blank" style="font-weight: bold; text-decoration: underline;">[Download PDF Slides]</a>
      </td>
    </tr>
  </tbody>
</table>

---

## Prerequisites
To get the most out of this tutorial, attendees are recommended to have:
* **Basic Knowledge:** Familiarity with Knowledge Graphs and standard embedding frameworks (e.g., TransE, RotatE).
* **Programming:** Familiarity with Python, PyTorch, or Deep Graph Library (DGL).
* **Hardware (Optional):** A laptop with access to Google Colab if you wish to follow along with the hands-on code examples.