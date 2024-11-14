# MedBench

CliMedBench is a comprehensive  benchmark with 14 expert-guided core clinical scenarios. It comprises 33,735 questions derived from real-world medical reports of top-tier tertiary hospitals and authentic examination exercises.

This repository contains supplementary information of the paper [*CliMedBench: A Large-Scale Chinese Benchmark for Evaluating Medical Large Language Models in Clinical Scenarios*](https://arxiv.org/abs/2410.03502).

## Scenarios Descriptions

- **In-hospital Diagnosis (Period \#1) (ID\#1)**: The first stage of patient consultation, physicians should formulate a tentative diagnosis from the patient's presenting symptoms and choose the most appropriate diagnostic test to confirm the condition.

- **In-hospital Diagnosis (Period #2) (ID#2)**: The second stage of patient consultation, physicians need to diagnose patients' diseases by their clinical data and examination results.

- **In-hospital Diagnosis (Period #3) (ID#3):** The third stage of patient consultation, physicians need to ascertain the appropriate treatment for patients by evaluating their diseases and presenting symptoms, which may involve surgical intervention or pharmacotherapy.

- **In-hospital Diagnosis (Period #4) (ID#4):** The fourth stage of patient consultation, the patient has recuperated, necessitating the physician to formulate discharge advice that considers the patient's admission and discharge statuses, alongside the timeline of diagnosis and treatment.

- **Basic Knowledge Test (BKT)**: Evaluating the LLMs' ability to apply basic medical knowledge.

- **False Info Test (FIT)**: Investigates the propensity of LLMs to generate factually inconsistent responses by presenting it with a medical query alongside an erroneous reference answer and prompting it for an explanation.

- **False Treatment Test (FTT)**: Discerns whether the LLMs recognizes the inaccuracy of the provided choices or merely generates a response that contradicts the facts by providing a query where the accurate response is "none of the above options are correct".

- **Wrong Treatment Detection(WTD)**: Require LLMs to express an opinion medical texts with toxicity.

- **Discharge Summary (DS)**: Supply the LLMs with a patient's medical record encompassing admission diagnosis, diagnostic and therapeutic course, surgical procedure, and intraoperative observations and request LLMs to generate a discharge summary.

- **Medicine Consultation (MC)**: Input patient symptomatology to the LLMs to identify therapeutically effective drugs from a list of alternatives. These drugs encompass agents with potential therapeutic mismatches, contraindications pertinent to the patient's clinical status, and risks of dosage inaccuracies.

- **Surgical Steps Organization (SSO)**: Block out key procedural steps in surgery and task LLMs with deducing their proper sequence through logical reasoning.

- **Clinical Pathway Reasoning (CPR)**: Disrupting the clinical pathway of patients and task LLMs with deducing their proper sequence through logical reasoning.

- **Keyword Extraction (KE)**: Presenting LLMs with medical paper abstracts and instructing them to identify keywords.

- **Case Summary (CS)**: Input a consultation report containing the patient's self-reported illness narrative, disease duration, and pharmacological history. Requires the LLMs to generate a succinct abstract of the record.

## Baselines & Results

To assess the state-of-the-art, we conduct evaluations using CliMedBench of 11 representative LLMs from both the general and medical domains. The metrics for each scenarios is marked in the table.

Main results:

![](C:\Users\欧阳泽田\AppData\Roaming\marktext\images\2024-11-14-13-52-09-image.png)



## Metadata and Examples

Please refer to the [`example/`](example/) directory.

## Contact

If you have any questions, please post a Github issue or email the authors.

## Citation

```bibtex
@misc{ouyang2024climedbenchlargescalechinesebenchmark,
      title={CliMedBench: A Large-Scale Chinese Benchmark for Evaluating Medical Large Language Models in Clinical Scenarios}, 
      author={Zetian Ouyang and Yishuai Qiu and Linlin Wang and Gerard de Melo and Ya Zhang and Yanfeng Wang and Liang He},
      year={2024},
      eprint={2410.03502},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2410.03502}, 
}
```
