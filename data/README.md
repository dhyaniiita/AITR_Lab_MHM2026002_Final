# Data Access & Description

The dataset used in this experiment is `qiaojin/PubMedQA` (pqa_labeled).
*   **Access:** Openly accessible via the HuggingFace Datasets library.
*   **Loading:** The script dynamically downloads the required stratified sample (30 instances) using `datasets.load_dataset('qiaojin/PubMedQA', 'pqa_labeled')`. No raw restricted data is stored locally.
