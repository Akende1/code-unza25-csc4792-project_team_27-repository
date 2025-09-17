# 1. Business Understanding

## Problem Statement

Wikipedia serves as a widely accessible knowledge repository, however the quality and completeness of articles vary. For Zambian topics, many articles remain underdeveloped, lacking depth, proper structure, sufficient references, and multimedia elements. This limits the availability of reliable, comprehensive information about Zambia for both local and global audiences.

Currently the process of identifying incomplete Zambian articles is largely manual, relying on editor intuition, quality assessments, and community discussions. This approach is time-consuming, inconsistent, and insufficient for  addressing the most critical content gaps. Without a scalable method to assess and prioritize articles, valuable editing efforts may be misdirected, leaving important topics underrepresented.

The core problem is the absence of an automated, consistent, and accurate system to determine and classify the completeness of Zambian Wikipedia pages. By analyzing text structure, metadata, and content coverage, such a system could classify articles according to Wikipedia’s quality scale and highlight key areas for improvement. This would enable editors to focus on the most impactful updates, improve the overall quality of Zambian content, and ensure that readers have access to well-developed, trustworthy information.

Solving this problem benefits multiple stakeholders: Wikipedia editors seeking guidance on where to contribute, WikiProject Zambia aiming to raise overall article standards, researchers and educators relying on accurate information, and the general public seeking a richer understanding of Zambia.


## Objectives and success criteria

### 1.1 Primary Objectives

We will build a classification model for:

**Objective 1: Article Classification System**
Develop a system to automatically classify Zambian Wikipedia articles into established quality levels based on Wikipedia’s quality scale:

- **Stub (Level 0)**: <100 words, ≤2 sections, very few/no internal links.

- **Basic (Level 1)**: 100–249 words, ≥2 sections, minimal structure.

- **Intermediate (Level 2)**: 250–399 words, ≥3 sections, ≥15 internal links, some structure and references.

- **Detailed (Level 3)**: 400–799 words, ≥4 sections, ≥30 internal links, well-structured with good linking.

- **Very Comprehensive (Level 4)**: ≥800 words, ≥5 sections, ≥50 internal links, highly structured, extensive references.

- **Featured Article (Level 5):** Exemplary standard, exceptional writing, comprehensive coverage.

*custom scale used for yhe purposes of this project.*

**Objective 2: Content Gap Identification**  
Identify missing or underdeveloped elements within articles categorized as:  
- Structural gaps (missing sections)  
- Content gaps (missing topics)  
- Reference gaps (unreliable sources)  
- Multimedia gaps (missing images, maps, diagrams)

**Objective 3: Actionable Insights Generation**  
Provide specific improvement recommendations, including:  
- Priority ranking of articles needing attention  
- Article-specific suggestions for enhancement  
- Content templates for common article types  
- Reference improvement strategies

### 1.2 Secondary Objectives
- Create a reusable assessment framework adaptable to other countries/topics.  
- Establish baseline metrics to track future Wikipedia content improvements.  
- Produce educational resources to guide editors on quality standards.

## 2. Success Criteria & Metrics

### 2.1 Primary Success Metrics
**Metric 1: Classification Accuracy**  
- **Target:** ≥85% accuracy in classifying articles.  
- **Measurement:** Compare automated classifications against human-rated articles using cross-validation and confusion matrix analysis.

**Metric 2: Gap Identification Accuracy**  
- **Target:** Correctly flag the top 20 most incomplete Zambian articles.  
- **Measurement:** Validate with expert review and compare with community consensus.

### 2.2 Secondary Success Metrics
**Model Performance Metrics**  
- **Precision:** Minimize false positives (overrating article quality).  
- **Recall:** Minimize false negatives (underrating article quality).  
- **F1-Score:** Balanced metric for each quality level.  
- **Cohen’s Kappa:** Measure agreement between model and human raters.

**Business Impact Metrics**  
- **Usability:** Wikipedia editors can easily interpret and act on recommendations.  
- **Efficiency:** Reduced time needed to identify priority improvement opportunities.  
- **Coverage:** Percentage of Zambian articles assessed by the system.

---

## 3. Validation Methods
**Expert Review**  
- Recruit 3–5 experienced Wikipedia editors.  
- Have them manually assess 50 randomly selected articles.  
- Compare their assessments with model output to measure agreement.

**Community Feedback**  
- Share results with WikiProject Zambia members.  
- Gather qualitative feedback on usefulness, accuracy, and priorities.  
- Apply feedback to refine the model and recommendations.

---

## 4. Data Mining Goals

**Automated Quality Classification**

Build a supervised classification model to automatically assign Zambian Wikipedia articles to one of six quality levels (Stub, Start, C-Class, B-Class, Good Article, Featured Article) based on Wikipedia’s quality scale.

- Content Gap Detection

Use text mining and metadata analysis to identify missing sections, low reference counts, insufficient word count, and lack of multimedia.

- Improvement Recommendation Generation

Develop a rule-based recommendation system that generates actionable suggestions for editors based on detected gaps (e.g., “Add references to support claims,” “Include an infobox,” “Expand the history section”).
