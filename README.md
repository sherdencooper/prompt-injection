# Custom GPT Security Analysis

## Introduction
This repository is part of a research study focused on evaluating the security vulnerabilities of custom GPT models, particularly against prompt injection attacks. Our paper, titled "Customized but Compromised: Assessing Prompt Injection Risks in User-Designed GPTs," details our methodology, findings, and implications for GPT security.

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
