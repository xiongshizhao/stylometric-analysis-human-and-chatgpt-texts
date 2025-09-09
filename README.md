# Stylometric Approaches to Authorship Attribution: Distinguishing Human-Written and ChatGPT-4o-mini Generated Texts
This repository contains the code, data, and results for a stylometric study on authorship attribution.  
The project investigates whether function-word-based stylometry can reliably distinguish human-written essays from ChatGPT-4o-mini generated texts. We evaluate three classifiers and examine how essay representation, text length, training data size, and topic relevance affect classification performance.  


### Authors:
- Jingqi He  
  Email: [j.he-40@sms.ed.ac.uk](mailto:j.he-40@sms.ed.ac.uk)
- Rongzhi Chen
  Email: [r.chen-52@sms.ed.ac.uk](mailto:r.chen-52@sms.ed.ac.uk)
- Shizhao Xiong  
  Email: [s.xiong-8@sms.ed.ac.uk](mailto:s.xiong-8@sms.ed.ac.uk)

### Supervisor:
- Gordon J. Ross, Reader at the University of Edinburgh  
  Email: [gordon.ross@ed.ac.uk](mailto:gordon.ross@ed.ac.uk)

---

### Project Overview  

This study addresses four research questions in authorship attribution:  

1. Whether human essays should be treated as a single aggregated class or as distinct authorial voices.  
2. How essay length influences classifier performance.  
3. How performance shifts when training data is limited.
4. Whether classifiers generalise across topics or rely on topic-specific features.  

---

### Repository Structure  

**Code/**  
R scripts for data preprocessing, feature extraction, classifier training, and evaluation.  

**Data/**  
- `GPTessays.zip`: ChatGPT-4o-mini generated essays.  
- `humanessays.zip`: Human-authored essays.  
- `functionwords.zip`: Function word counts and essay titles.  

**Results/**  
Organised outputs and figures from each of the four studies.  

**Figures/**  
Plots and visualisations illustrating classifier performance and study findings.  

---

### Studies Conducted  

1. **Study 1 – Aggregated vs. Individual Treatment of Human Essays**  
   Comparison of classification when human essays are treated as one group versus as distinct authorial styles.  

2. **Study 2 – Impact of Essay Length**  
   Evaluation of classifier performance on full length essays versus 200-word excerpts.  

3. **Study 3 – Impact of Training Data Size**  
   Analysis of how reducing the proportion of training essays (100%, 50%, 20%, 10%) influences classifier robustness.  

4. **Study 4 – Influence of Topic Relevance**  
   Assessment of whether classification depends on topic-specific cues, comparing within-topic training, unrelated-topic training, and cross-topic training.  

---

### Classifiers Evaluated  

- **Burrows’ Delta**
- **Random Forest**  
- **Support Vector Machines**  

Performance was assessed using accuracy, precision, recall, and F1 score.  

---

### How to Use  

1. **Prepare Data**  
   - Extract `GPTessays.zip`, `humanessays.zip`, and `functionwords.zip`.  

2. **Run Analyses**  
   - Use the R scripts in the `Code/` folder.  
   - Example usage:  
     - `form_of_data.R` → Study 1  
     - `WordLength.R` → Study 2  
     - `traindata_size.R` → Study 3  
     - `Except topic.R`, `Except_only_topic.R` and `OnlyTopic.R` → Study 4  

---

### Future Directions  

- Extend the dataset to include texts from other large language models.  
- Investigate hybrid authorship (human + AI collaboration).  
- Explore ensemble methods to improve robustness across topics and text lengths.  

---

### Additional Information  

For inquiries or further details, please contact the research team or the supervisor.  
