# ICU Prognosis using Explainable Generative Pre-trained Transformers from Electronic Health Records

Author: Diego Saenz

## Abstract

The surging adoption of electronic health records (EHR) systems produces ever-larger collections of comprehensive historical data. Clinicians, however, struggle to absorb these large amounts of patient information for immediate decisions. Medical institutions could also be prepared to administer beds and spaces efficiently for incoming patients if the severity of their stay is likely known. Utilizing large-scale EHR data for an early prediction of patient outcomes should lead to improved diagnosis, treatment, enhanced management of medical resources, and prompt intervention. Moreover, predicting outcomes for admitted patients to the intensive care unit is even more critical than other patient populations. Classical machine learning algorithms and deep recurrent neural networks have failed to comprehend large sequences of information from a person's entire clinical history. Recently, transformers-based networks have shown exciting results when working with large-scale longitudinal electronic health records. However, these advancements are limited to specific applications and introduce challenges at deployment because of massive model parameter sizes. We show how a transformer network framework built on sequence-to-sequence modeling is capable of understanding EHR data, generatively learning from it, and selecting influential patient data records to perform diverse tasks. Here, we propose PICUT, a novel, efficient and explainable transformer-based framework to aggregate patients' EHR information and produce a broader and global medical language to understand the patients' history. We build and evaluate the solution on 250 thousand patient records from the publicly available MIMIC-IV v1.0 dataset. We fine-tune the proposed solution to predict multiple patient outcomes related to heart failure, length of hospitalization, and re-admission using 50 thousand patient records. We show how our architecture provides state-of-the-art performance while being three times smaller in parameter size than most transformer-based EHR frameworks to-date, making it more suitable for deployment. Our PICUT architecture is able to explain its decisions by linearly approximating the classification boundary for a meaningful input feature summary of important elements in the patients' history.

## Data

The data for this study was obtained from the Medical Information Mart for Intensive Care (MIMIC-IV) v1.0. It can be found [here](https://physionet.org/content/mimiciv/1.0/).

## Installation

Run the following command in a python 3.6 or older environment:

```
pip install -r requirements.txt
```

## Training

You may run the python scripts in the pretraining and finetuning folders with the input data. All parameters are explain in the respective scripts.
