# Nos Instagram Analyzer AI v1.0 🤖
![banner image](https://github.com/anezatra/nos-ai/blob/main/banner.jpg)
## What is Nos AI used for?
**Nos AI is an artificial intelligence software that utilizes the GPT-2 language model to analyze Instagram users in real-time at specified intervals and communicates this information to the user. For instance, Nos attempts to find out whom an Instagram user most recently sent a request to or where a specific account's name has appeared, either in posts or biographies, by examining the accounts followed by the target user. All these operations are conducted by leveraging Instagram APIs. To use the program, Nos needs to log in to any account.**
[Click to watch the video of the program.](https://www.youtube.com/watch?v=qaDWwOpjV3M)
## How the GPT-2 Language model works 🛠
**GPT-2 (Generative Pre-trained Transformer 2) is a language model pretrained on a large corpus of text data. This model processes and understands text data using transformer neural networks. With its self-attention mechanism, it can generate new text sequentially starting from a given input. During text generation, GPT-2 evaluates the possible continuation of each word or character and selects the most probable one. Additionally, it can be utilized in various language tasks such as text completion, translation, summarization, and question-answering, yielding successful results. These fundamental principles of operation rely on the model's ability to learn complex language patterns by leveraging large-scale data and computational power.** <br/>
![Banner](https://github.com/anezatra/nos-ai/blob/main/working.jpg)
## Use of GPT-2 in Nos AI ⚙️
**The GPT-2 model used by Nos was trained on a small dataset consisting of specific actions. The current GPT-2 Model has 124 million hyperparameters. It generates text based on users' actions on their accounts. Nos GPT2 first collects the accounts followed by the target account. During the initial collection, it perceives them as newly followed accounts and records the initially checked users. Later on, it checks whether the analyzed user's name appears in the accounts they follow. For this purpose, it focuses on the writings, comments, and biographies of the accounts followed by the analyzed user. If the analyzed user's name is found among the followed accounts, Nos promptly informs you. Subsequently, it attempts to collect the open-source data of the analyzed user from the internet, completing the initial check this way. In the next analysis, if the analyzed user has followed someone new within the specified time frame, Nos directly informs you about this person and analyzes all their information. Below is a ascii visual representation of this process:**
```
-------------------------       -------------------------       ---------------------------------------------
| Target access control |   ═>  | Analyzing followings  |   ═>  | Look for evidence in those being followed | 
-------------------------       -------------------------       ---------------------------------------------
                                                                                    ‖
                                                                                    ‖
                    ╔═══════════════════════════════════════════════════════════════╝
                    ‖                           GPT-2 NOS
                    ‖
------------------------------------------------        --------------------------------------------------------------------
| Check out followers posts for more evidence. |   ═>   | Finding open source data of the target with the Google algorithm |
------------------------------------------------        --------------------------------------------------------------------        
                                                                                    ‖                                                                                                                                         ‖
                                                                                    ‖
                    ╔═══════════════════════════════════════════════════════════════╝
                    ‖                           GPT-2 NOS
                    ‖
------------------------------------        --------------------------
| Catch Target's users you request |   ═>   |  Back to the beginning |
------------------------------------        --------------------------
```
## Nos AI Models 📝
**GPT-1 NOS 117M: Soon ❌** <br/>
**GPT-2 NOS 124M: Click to access the [model](https://huggingface.co/anezatra/gpt2-nos-124M). ✔️** <br/>
**GPT-2 NOS 355M: Soon ❌** <br/>

## All modules 🔍
```
user_tracking_mode_ai       This module analyzes the target using the gpt2 module of Nos. 
user_tarcking_mode_basic    This module simply analyzes the target using the normal model of Nos.
```
## Example usage ⛏

```
nos > 1

[INFO]: Module loaded: user_tracking_mode_ai
--------------------------------------------

nos(user_tracking_mode_ai)> set tokenizer anezatra/gpt2-nos-124M

[!] set TOKENIZER => anezatra/gpt2-nos-124M

nos(user_tracking_mode_ai)> set model anezatra/gpt2-nos-124M

[!] set MODEL => anezatra/gpt2-nos-124M

nos(user_tracking_mode_ai)> set username example

[+] set USERNAME => example

nos(user_tracking_mode_ai)> set password 1234

[+] set PASSWORD => 1234

nos(user_tracking_mode_ai)> set target target_account

[+] set TARGET => target_account

nos(user_tracking_mode_ai)> set time 30

[+] set TIME => 30

nos(user_tracking_mode_ai)> set amount 100

[+] set AMOUNT => 100

nos(user_tracking_mode_ai)> run
```
**Note: If your computer does not support Cuda or is not powerful, use Module 2**
## How to download 💡
**You can download nos directly by saying** <br/><br/>
` pip install -r requirements.txt `
## or <br/>
` python -m pip install -r requirements.txt ` <br/>
## Required python version 📌
` python 3.x `
## Required instagram API module 🛠️
**In order to use the program without any errors, the instagrapi download the latest version. You can download it with the requirements file or download it with the pip command**
## About 🚀
**My gmail adress: anezatra@gmail.com** <br/>


