---
layout: default
title: CKGE-FMOC Tutorial
---

<style>
  /* Hides the automatic theme header and the blue link at the top */
  .page-header {
    display: none !important;
  }
  
  /* Container to keep the main content clean and add top spacing */
  .main-content {
    padding-top: 40px !important;
  }

  /* Flexbox alignment for the logo and title */
  .title-container {
    display: flex;
    align-items: center;
    gap: 20px;
    margin-bottom: 20px;
  }

  .title-logo {
    height: 90px; /* Adjust the height to match your logo's proportions */
    width: auto;
    flex-shrink: 0;
  }

  .main-title {
    margin: 0 !important;
    font-size: 2rem !important;
    line-height: 1.25 !important;
    font-weight: 700;
    color: #1f2937;
  }
</style>

<div class="title-container">
  <img src="images/logo.png" alt="CKGE-FMOC Logo" class="title-logo">
  <h1 class="main-title">CKGE-FMOC: Continual Knowledge Graph Embedding: Foundations, Methods, and Open Challenges</h1>
</div>

<div style="text-align: center; margin: 30px 0; line-height: 1.8;">
  <h3 style="margin-bottom: 10px; color: #1f2937;">A Tutorial at the <strong>25th International Semantic Web Conference (ISWC 2026)</strong></h3>
  <span style="display: block; font-size: 1.05rem;"><strong>Date:</strong> October 25 - 29, 2026</span>
  <span style="display: block; font-size: 1.05rem;"><strong>Venue:</strong> The Nicolaus Hotel, Bari, Italy</span>
</div>


---

## Abstract
Knowledge Graph Embeddings (KGEs) provide fixed-length **vector representations** of entities and relations within a Knowledge Graph (KG), enabling a wide variety of downstream tasks over KGs. However, **real-world KGs are dynamic**, and continuously evolve with the addition of new entities, relations, and facts. Updating embeddings to reflect this growth without constantly retraining models from scratch, which is costly, presents a significant challenge. While generic continual learning approaches, such as fine-tuning, can be applied, they often fail to leverage the **unique properties of KGs**.

Since late 2023, a new research direction, Continual Knowledge Graph Embedding (CKGE), has emerged to address this limitation. There is a **growing interest in the field**, with nearly twenty specialized methods proposed in recent years. This tutorial aims to first introduce the **fundamentals** and motivation behind KGEs, and then provide a comprehensive **overview of CKGE**. We present a structured **categorization** of state-of-the-art approaches, highlighting their underlying principles and differences, as well as the evaluation protocols and metrics specific to continual settings. In addition, we examine the problem of **catastrophic forgetting**, analyzing its causes in evolving KGs and its impact on model performance. The tutorial concludes by discussing **open challenges and promising directions** for future research in CKGE.

---

## Presenters

<div style="display: flex; flex-direction: column; gap: 30px; margin-top: 20px;">
  
  <div style="display: flex; align-items: center; gap: 20px; flex-wrap: wrap;">
    <img src="images/presenter1.jfif" alt="Presenter 1 Name" style="width: 150px; height: 150px; border-radius: 50%; object-fit: cover; flex-shrink: 0; border: 2px solid #ddd;">
    <div style="flex: 1; min-width: 250px;">
      <h3 style="margin-top: 0;">Gerard Pons</h3>
      <p style="margin: 5px 0;"><em>Universitat Politècnica de Catalunya</em></p>
      <p style="margin: 0;">Gerard Pons is a last-year PhD candidate in Computing from Universitat Politècnica de Catalunya (UPC), where he works on dynamic KGs, exploring topics such as CKGE and Entity Disambiguation. In addition to his research, he is also an adjunct professor at the Faculty of Informatics of Barcelona (FIB) at the UPC. He has been researching KGEs since 2021, with a particular focus on CKGE in recent years.</p>
    </div>
  </div>

  <div style="display: flex; align-items: center; gap: 20px; flex-wrap: wrap;">
    <img src="images/presenter2.jfif" alt="Presenter 2 Name" style="width: 150px; height: 150px; border-radius: 50%; object-fit: cover; flex-shrink: 0; border: 2px solid #ddd;">
    <div style="flex: 1; min-width: 250px;">
      <h3 style="margin-top: 0;">Anna Queralt</h3>
      <p style="margin: 5px 0;"><em>Universitat Politècnica de Catalunya</em></p>
      <p style="margin: 0;">Anna Queralt is an Associate Professor at UPC, where she leads the Data-intensive Technologies and Knowledge Systems (DTAK) research group. She was a Senior Researcher at the Barcelona Supercomputing Center (BSC) from 2012 to 2024, leading the Distributed Object Management research line. Her research interests include data life cycle management, knowledge bases, and graph representation learning.</p>
    </div>
  </div>

</div>

---

<h2>Schedule</h2>

<table style="width: 100%; border-collapse: collapse; text-align: left;">
  <thead>
    <tr style="background-color: #f6f8fa; border-bottom: 2px solid #d0d7de;">
      <th style="padding: 12px; width: 25%;">Session</th>
      <th style="padding: 12px; width: 20%;">Time</th>
      <th style="padding: 12px; width: 55%;">Program & Materials</th>
    </tr>
  </thead>
  <tbody>
    <tr style="border-bottom: 1px solid #d0d7de;">
      <td style="padding: 12px; font-weight: bold; background-color: #fafafa;">Opening</td>
      <td style="padding: 12px;">09:00 - 09:05</td>
      <td style="padding: 12px;">
        <strong>Introduction and Motivation</strong>
      </td>
    </tr>
    <tr style="border-bottom: 1px solid #d0d7de;">
      <td style="padding: 12px; font-weight: bold; background-color: #fafafa;">Session 1</td>
      <td style="padding: 12px;">09:05 - 09:45</td>
      <td style="padding: 12px;">
        <strong>Knowledge Graph Embeddings</strong><br>
        Foundations of Knowledge Graph Embeddings.
        <br><a href="slides/session1_kge_foundations.pdf" target="_blank" style="font-weight: bold; text-decoration: underline;">[Download PDF Slides]</a>
      </td>
    </tr>
    <tr style="border-bottom: 1px solid #d0d7de;">
      <td style="padding: 12px; font-weight: bold; background-color: #fafafa;">Hands-On 1</td>
      <td style="padding: 12px;">09:45 - 10:10</td>
      <td style="padding: 12px;">
        <strong>Interactive Session on KGEs</strong><br>
        Practical exercises and experimentation with Knowledge Graph Embeddings.
        <br><a href="notebooks/kge_hands_on.ipynb" target="_blank" style="font-weight: bold; text-decoration: underline;">[Open Notebook]</a>
      </td>
    </tr>
    <tr style="border-bottom: 1px solid #d0d7de;">
      <td style="padding: 12px; font-weight: bold; background-color: #fafafa;">Session 2</td>
      <td style="padding: 12px;">10:10 - 10:40</td>
      <td style="padding: 12px;">
        <strong>Continual Knowledge Graph Embedding</strong><br>
        Preliminaries of CKGE.
        <br><a href="slides/session2_ckge_preliminaries.pdf" target="_blank" style="font-weight: bold; text-decoration: underline;">[Download PDF Slides]</a>
      </td>
    </tr>
    <tr style="border-bottom: 1px solid #d0d7de;">
      <td style="padding: 12px; font-weight: bold; background-color: #fafafa;">Break</td>
      <td style="padding: 12px;">10:40 - 11:10</td>
      <td style="padding: 12px;">
        <strong>Coffee Break</strong>
      </td>
    </tr>
    <tr style="border-bottom: 1px solid #d0d7de;">
      <td style="padding: 12px; font-weight: bold; background-color: #fafafa;">Session 3</td>
      <td style="padding: 12px;">11:10 - 11:35</td>
      <td style="padding: 12px;">
        <strong>Categorization of CKGE Methods</strong><br>
        Taxonomy and main building blocks.
        <br><a href="slides/session3_ckge_taxonomy.pdf" target="_blank" style="font-weight: bold; text-decoration: underline;">[Download PDF Slides]</a>
      </td>
    </tr>
    <tr style="border-bottom: 1px solid #d0d7de;">
      <td style="padding: 12px; font-weight: bold; background-color: #fafafa;">Session 4</td>
      <td style="padding: 12px;">11:35 - 12:00</td>
      <td style="padding: 12px;">
        <strong>Challenges in CKGE</strong><br>
        From embedding initialization to entity interference.
        <br><a href="slides/session4_ckge_challenges.pdf" target="_blank" style="font-weight: bold; text-decoration: underline;">[Download PDF Slides]</a>
      </td>
    </tr>
    <tr style="border-bottom: 1px solid #d0d7de;">
      <td style="padding: 12px; font-weight: bold; background-color: #fafafa;">Hands-On 2</td>
      <td style="padding: 12px;">12:00 - 12:45</td>
      <td style="padding: 12px;">
        <strong>Interactive Session on CKGE Training and Evaluation</strong><br>
        Practical exercises on continual learning for knowledge graphs.
        <br><a href="notebooks/ckge_hands_on.ipynb" target="_blank" style="font-weight: bold; text-decoration: underline;">[Open Notebook]</a>
      </td>
    </tr>
    <tr>
      <td style="padding: 12px; font-weight: bold; background-color: #fafafa;">Closing</td>
      <td style="padding: 12px;">12:45 - 12:50</td>
      <td style="padding: 12px;">
        <strong>Discussion &amp; Closing</strong>
      </td>
    </tr>

  </tbody>
</table>



---

## Prerequisites
To get the most out of this tutorial, attendees are recommended to have:
* **Basic Knowledge:** Familiarity with Knowledge Graphs and Machine Learning.
* **Programming:** Familiarity with Python.
* **Hardware (Optional):** A laptop with access to Google Colab if you wish to follow along with the hands-on code examples.

Familiarity with representation learning or embedding methods is helpful but not strictly required, as key concepts will be introduced during the tutorial.

