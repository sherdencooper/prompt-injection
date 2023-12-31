# Custom GPT Security Analysis

## Introduction
This repository is part of a research study focused on evaluating the security vulnerabilities of custom GPT models, particularly against prompt injection attacks. Our paper, titled "[Assessing Prompt Injection Risks in 200+ Custom
GPTs](https://arxiv.org/abs/2311.11538)" details our methodology, findings, and implications for GPT security.

## Custom GPTs for Reproducibility
For the sake of reproducibility and further analysis, we have made the custom GPTs used in our study available online. You can access them through the following links:

- [System Prompt Extraction without Code Interpreter](https://chat.openai.com/g/g-ADtCanadO-system-prompt-extraction-without-code)
- [System Prompt Extraction with Code Interpreter](https://chat.openai.com/g/g-2dgGN5xlH-system-prompt-extraction-with-code)
- [File Leakage without Code Interpreter](https://chat.openai.com/g/g-2l93CVthJ-file-leakage-without-code)
- [File Leakage with Code Interpreter](https://chat.openai.com/g/g-Wj66sRmK8-file-leakage-with-code)

## Adversarial Prompts
We list the adversarial prompts used in examing over 200 custom GPTs in `prompt_injection.md`.

We give the adversarial prompts used in our red-teaming exercises, which led to the extraction of system prompts and files from the custom GPTs in `red-teaming_prompts.md`.

## Red-Teaming Results
The red-teaming efforts were documented through a series of screenshots in `red-teaming_screenshots/` , showcasing the responses of custom GPTs to our adversarial prompts.

## Citation
If you find our work useful, please cite our paper:
```
@article{yu2023assessing,
  title={Assessing Prompt Injection Risks in 200+ Custom GPTs},
  author={Yu, Jiahao and Wu, Yuhang and Shu, Dong and Jin, Mingyu and Xing, Xinyu},
  journal={arXiv preprint arXiv:2311.11538},
  year={2023}
}
```

## FQA
1. Could you share the experiment data or the target custom GPT list?
   
   We are afraid that we cannot share them. As we stated in our paper, we deleted all extracted information after the experiment to avoid ethical concerns. Similarly, we cannot provide the list of the target GPTs.
2. I tried the red-teaming prompts but did not yield the same results shown in the screenshots.

   Due to the sampling nature of GPTs, you may get different results even when you use the same prompts in the web interference. Thus, simply retrying may help. However, we did notice the improved prompt injection robustness by Nov 16 that some red-teaming prompts could not succeed even after 5 trials. This is potentially due to some updates of OpenAI.
