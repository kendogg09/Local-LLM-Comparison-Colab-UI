# Local LLM Comparison & Colab Links (WIP)
Compare the performance of different LLM that can be deployed locally on consumer hardware. The expected good response and scores are generated by GPT-4.

For your convenience, I have made the colab notebooks with oobabooga's text generation webui for trying out the models (I'm creating GPTQ colab notebooks as llama.cpp has made some breaking changes). You can find the links in the table below. For models supported by GPT4ALL, you can simply use their one-click installer and download the models there.

## Models tested & average score:
These models work better among the models I tested on my hardware (i5-12490F, 32GB RAM):
(Note: Because llama.cpp has made some breaking changes to the support of older ggml models. Some older ggml versions listed below may not work properly on current llama.cpp. But there should be GPTQ equivalents or newer ggml versions for the models.)

| Model                                                                           | Avg_Score | Colab_Link                                                                                                                                                                                                                                                | Date_Added | Link                                                                    |
| :------------------------------------------------------------------------------ | :-------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :--------- | :---------------------------------------------------------------------- |
| wizard-vicuna-13B.ggml.q4_0 (using llama.cpp)                                   | 9.31      | <a target="_blank" href="https://colab.research.google.com/github/Troyanovsky/Local-LLM-comparison/blob/main/wizard_vicuna_13B_GPTQ.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>                  | 2023/05/07 | https://huggingface.co/TheBloke/wizard-vicuna-13B-GGML                  |
| wizardLM-7B.q4_2 (in GPT4All)                                                   | 9.31      | No                                                                                                                                                                                                                                                        | 2023/05/07 | https://gpt4all.io/models/ggml-wizardLM-7B.q4_2.bin                     |
| manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui)             | 8.31      | <a target="_blank" href="https://colab.research.google.com/github/Troyanovsky/Local-LLM-comparison/blob/main/manticore_13b_chat_pyg_GPTQ.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>             | 2023/05/24 | https://huggingface.co/TheBloke/manticore-13b-chat-pyg-GPTQ             |
| mpt-7b-chat (in GPT4All)                                                        | 8.25      | No                                                                                                                                                                                                                                                        | 2023/05/11 | https://gpt4all.io/models/ggml-mpt-7b-chat.bin                          |
| wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) | 8.06      | <a target="_blank" href="https://colab.research.google.com/github/Troyanovsky/Local-LLM-comparison/blob/main/wizard_lm_uncensored_13b_GPTQ_4bit_128g.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> | 2023/05/19 | https://huggingface.co/4bit/WizardLM-13B-Uncensored-4bit-128g           |
| vicuna-13b-1.1-q4_1 (in GPT4All)                                                | 7.94      | No                                                                                                                                                                                                                                                        | 2023/05/07 | https://gpt4all.io/models/ggml-vicuna-13b-1.1-q4_2.bin                  |
| koala-13B-4bit-128g.GGML (using llama.cpp)                                      | 7.88      | No                                                                                                                                                                                                                                                        | 2023/05/07 | https://huggingface.co/TheBloke/koala-13B-GPTQ-4bit-128g-GGML           |
| Manticore-13B-GPTQ (using oobabooga/text-generation-webui)                      | 7.81      | <a target="_blank" href="https://colab.research.google.com/github/Troyanovsky/Local-LLM-comparison/blob/main/Manticore_13B_GPTQ.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>                                                                                                                                                                                                                                                        | 2023/05/23 | https://huggingface.co/TheBloke/Manticore-13B-GPTQ                      |
| stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui)        | 7.81      | No                                                                                                                                                                                                                                                        | 2023/05/12 | https://huggingface.co/TheBloke/stable-vicuna-13B-GPTQ                  |
| gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp)                                   | 6.5625    | No                                                                                                                                                                                                                                                        | 2023/05/07 | https://huggingface.co/Bradarr/gpt4-x-alpaca-13b-native-ggml-model-q4_0 |
| mpt-7b-instruct                                                                 | 6.375     | No                                                                                                                                                                                                                                                        | 2023/05/12 | https://huggingface.co/TheBloke/MPT-7B-Instruct-GGML                    |
| gpt4all-j-v1.3-groovy (in GPT4All)                                              | 5.5625    | No                                                                                                                                                                                                                                                        | 2023/05/07 | https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin                |
|                                                                                 |           |                                                                                                                                                                                                                                                           |            |                                                                         |

Many thanks to:  
❤️ GPT4ALl: https://github.com/nomic-ai/gpt4all-chat  
❤️ llama.cpp: https://github.com/ggerganov/llama.cpp  
❤️ oobabooga text generation webui: https://github.com/oobabooga/text-generation-webui  
❤️ Colab webui inspired by camenduru: https://github.com/camenduru/text-generation-webui-colab/tree/main  
❤️ The Bloke for quantization of the models: https://huggingface.co/TheBloke  

## Questions and scores
Original responses can be found at: https://docs.google.com/spreadsheets/d/1ogDXUiaBx3t7EpMo44aaA6U6kLXX0x2tGRgLg8CISGs/edit?usp=sharing

### Question 1: Translate the following English text into French: "The sun rises in the east and sets in the west."  
Task Domain: Translation  
Expected Good Response: "Le soleil se lève à l'est et se couche à l'ouest."  
Explanation: This task tests the model's ability to understand and accurately translate text between languages.  
- wizardLM-7B.q4_2 (in GPT4All) : 10  
- gpt4all-j-v1.3-groovy (in GPT4All) : 1  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 9  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 10  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 8  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 10  
- mpt-7b-chat (in GPT4All) : 1  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 1  
- mpt-7b-instruct : 1  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 8  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 10  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 10  

### Question 2: Summarize the following text: "The water cycle is a natural process that involves the continuous movement of water on, above, and below the Earth's surface. It includes various stages like evaporation, condensation, precipitation, and runoff. This cycle plays a crucial role in maintaining Earth's water balance and supporting life."  
Task Domain: Summary  
Expected Good Response: "The water cycle is the continuous movement of water on Earth, crucial for maintaining water balance and supporting life."  
Explanation: This task evaluates the model's ability to extract the main points from a given text and generate a concise summary.  
- wizardLM-7B.q4_2 (in GPT4All) : 9  
- gpt4all-j-v1.3-groovy (in GPT4All) : 4  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 10  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 8  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 9  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 10  
- mpt-7b-chat (in GPT4All) : 10  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- mpt-7b-instruct : 5  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 1  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 9  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 9  

### Question 3: I want you to act as a senior software developer with deep knowledge in system design, frontend programming, and backend programming. Provide a high level design of a mental health journal app. Include the frontend and backend components. Do not write code.  
Task Domain: App Design  
Explanation: This task evaluates the model's ability to closely follow user's instruction for a complex task.  
- wizardLM-7B.q4_2 (in GPT4All) : 9  
- gpt4all-j-v1.3-groovy (in GPT4All) : 9  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 9  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 9  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 9  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 9  
- mpt-7b-chat (in GPT4All) : 9  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- mpt-7b-instruct : 7  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 9  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 9  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 10  

### Question 4: What are the main causes of the French Revolution according to this passage: "The French Revolution, which took place between 1789 and 1799, was rooted in financial crises, social inequality, and Enlightenment ideas."  
Task Domain: Abstractive Question Answering  
Expected Good Response: Financial crises, social inequality, and Enlightenment ideas.  
Explanation: This task tests the model's ability to understand the context and generate an answer in its own words.  
- wizardLM-7B.q4_2 (in GPT4All) : 10  
- gpt4all-j-v1.3-groovy (in GPT4All) : 10  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 10  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 5  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 10  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 10  
- mpt-7b-chat (in GPT4All) : 10  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- mpt-7b-instruct : 6  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 5  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 10  

### Question 5: In the following text, identify the two artists mentioned: "During the Renaissance, Leonardo da Vinci and Michelangelo were two of the most influential artists who created masterpieces that continue to inspire people today."  
Task Domain: Extractive Question Answering  
Expected Good Response: Leonardo da Vinci, Michelangelo  
Explanation: This task assesses the model's ability to extract specific information from a given text.  
- wizardLM-7B.q4_2 (in GPT4All) : 10  
- gpt4all-j-v1.3-groovy (in GPT4All) : 7  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 10  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 8  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 10  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 10  
- mpt-7b-chat (in GPT4All) : 6  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- mpt-7b-instruct : 9  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 10  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 10  

### Question 6: Determine the sentiment of this customer review: "I had a fantastic experience at this restaurant. The food was delicious, and the service was outstanding."  
Task Domain: Sentiment Analysis  
Expected Good Response: Positive  
Explanation: This task evaluates the model's ability to analyze text and identify the sentiment expressed.  
- wizardLM-7B.q4_2 (in GPT4All) : 10  
- gpt4all-j-v1.3-groovy (in GPT4All) : 10  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 10  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 10  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 10  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 10  
- mpt-7b-chat (in GPT4All) : 10  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- mpt-7b-instruct : 10  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 10  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 10  

### Question 7: Classify the following text into one of these categories: Sports, Technology, Health, or Politics: "Apple recently unveiled its latest iPhone, featuring a faster processor and improved battery life."  
Task Domain: Zero-shot Classification  
Expected Good Response: Technology  
Explanation: This task tests the model's ability to classify text into predefined categories without any prior training on the specific categories.  
- wizardLM-7B.q4_2 (in GPT4All) : 10  
- gpt4all-j-v1.3-groovy (in GPT4All) : 9  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 1  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 10  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 10  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 10  
- mpt-7b-chat (in GPT4All) : 10  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- mpt-7b-instruct : 10  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 10  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 10  

### Question 8: Complete the following sentence by filling in the blank: "The capital city of France is _______."  
Task Domain: Mask Filling  
Expected Good Response: Paris  
Explanation: This task assesses the model's ability to understand context and generate appropriate words to fill in missing information.  
- wizardLM-7B.q4_2 (in GPT4All) : 10  
- gpt4all-j-v1.3-groovy (in GPT4All) : 10  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 10  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 5  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 10  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 10  
- mpt-7b-chat (in GPT4All) : 10  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- mpt-7b-instruct : 10  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 10  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 10  

### Question 9: Write a rhyming couplet about nature.  
Task Domain: Poetry Generation  
Expected Good Response: "In nature's beauty, we find respite and grace,
A symphony of colors that time cannot erase."  
Explanation: This task tests the model's ability to generate creative and coherent text that adheres to specific constraints, such as rhyme and theme.  
- wizardLM-7B.q4_2 (in GPT4All) : 10  
- gpt4all-j-v1.3-groovy (in GPT4All) : 8  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 10  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 6  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 5  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 9  
- mpt-7b-chat (in GPT4All) : 9  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 5  
- mpt-7b-instruct : 4  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 9  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 6  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 8  

### Question 10: Based on the following statement, determine if the author's opinion is for or against nuclear energy: "Nuclear energy is a powerful source, but the potential risks and radioactive waste management issues make it a dangerous choice."  
Task Domain: Opinion Detection  
Expected Good Response: Against  
Explanation: This task evaluates the model's ability to understand and identify the author's stance or opinion on a specific topic.  
- wizardLM-7B.q4_2 (in GPT4All) : 10  
- gpt4all-j-v1.3-groovy (in GPT4All) : 4  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 10  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 9  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 6  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 10  
- mpt-7b-chat (in GPT4All) : 8  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- mpt-7b-instruct : 8  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 8  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 10  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 9  

### Question 11: Rewrite the following sentence in passive voice: "The dog chased the cat."  
Task Domain: Text Rewriting  
Expected Good Response: "The cat was chased by the dog."  
Explanation: This task tests the model's ability to manipulate and rewrite text according to specific grammatical requirements.  
- wizardLM-7B.q4_2 (in GPT4All) : 10  
- gpt4all-j-v1.3-groovy (in GPT4All) : 1  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 10  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 5  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 10  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 10  
- mpt-7b-chat (in GPT4All) : 10  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- mpt-7b-instruct : 8  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 10  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 10  

### Question 12: Use the retrieved context to answer a question. Context does not contain the answer. (Prompt too long. See spreadsheet for original prompt)
Task Domain: Document Question Answering  
Expected Good Response: "I don't know."  
Explanation: This task tests the model's ability to understand context and answer questions based on the information provided in the context.  
- wizardLM-7B.q4_2 (in GPT4All) : 10  
- gpt4all-j-v1.3-groovy (in GPT4All) : 1  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 1  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 1  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 10  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 10  
- mpt-7b-chat (in GPT4All) : 10  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- mpt-7b-instruct : 1  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 10  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 1  

### Question 13: Use the retrieved context to answer a question. Context contains the answer. (Prompt too long. See spreadsheet for original prompt)
Task Domain: Document Question Answering  
Expected Good Response: "["Semantic text search", "Generative question-answering", "Hybrid search", "Image similarity search", "Product recommendations"]"  
Explanation: This task tests the model's ability to understand context and answer questions based on the information provided in the context.  
- wizardLM-7B.q4_2 (in GPT4All) : 10  
- gpt4all-j-v1.3-groovy (in GPT4All) : 1  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 3  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 5  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 7  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 7  
- mpt-7b-chat (in GPT4All) : 8  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 3  
- mpt-7b-instruct : 10  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 8  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 1  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 7  

### Question 14: What is the square root of banana?
Task Domain: Mathematical Reasoning  
Expected Good Response: "The question is nonsensical, as square roots can only be calculated for numbers, not for objects or words like 'banana'."  
Explanation: This task tests the model's ability to recognize questions that are illogical or nonsensical and respond accordingly.  
- wizardLM-7B.q4_2 (in GPT4All) : 10  
- gpt4all-j-v1.3-groovy (in GPT4All) : 3  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 10  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 1  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 1  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 10  
- mpt-7b-chat (in GPT4All) : 8  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 2  
- mpt-7b-instruct : 1  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 1  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 2  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 9  

### Question 15: Extract the sender's name and address from the following text: "Dear Troy, Thanks for sharing your thoughts on document qa with Claude LLM and your comments on Tim's thoughts. My address is 5000 Forbes Ave, Pittsburgh, PA 15213. Best, Alex." Respond in JSON with one field for name and the other field for address.
Task Domain: Information Extraction  
Expected Good Response: {"name": "Alex","address": "5000 Forbes Ave, Pittsburgh, PA 15213"}  
Explanation: This task tests the model's ability to extract specific information (sender's name and address) from a given text and present the extracted information in a JSON format.  
- wizardLM-7B.q4_2 (in GPT4All) : 10  
- gpt4all-j-v1.3-groovy (in GPT4All) : 10  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 10  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 10  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 10  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 10  
- mpt-7b-chat (in GPT4All) : 10  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- mpt-7b-instruct : 5  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 10  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 10  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 9  

### Question 16: Given the following list of words. Categorize the words into 5 categories by similarity. Give each category a name. Respond in a python dictionary with key as the category name and value as a list of words in that category. List of words: ['Quagmire', 'Luminous', 'Melancholy', 'Perplexed', 'Jubilant', 'Enigmatic', 'Ambiguous', 'Ravenous', 'Obsolete', 'Tenacious', 'Euphoric', 'Wistful', 'Clandestine', 'Insidious', 'Inquisitive', 'Resilient', 'Surreptitious', 'Serendipity', 'Idiosyncratic', 'Juxtaposition']
Task Domain: Categorization  
Expected Good Response:  
{
  "Emotions": ['Melancholy', 'Jubilant', 'Euphoric', 'Wistful'],
  "Qualities": ['Luminous', 'Tenacious', 'Resilient'],
  "Mysterious": ['Quagmire', 'Enigmatic', 'Ambiguous', 'Clandestine', 'Surreptitious'],
  "Inquisitive": ['Perplexed', 'Inquisitive'],
  "Uncommon": ['Ravenous', 'Obsolete', 'Insidious', 'Serendipity', 'Idiosyncratic', 'Juxtaposition']
}  
Explanation: This task tests the model's ability to categorize a list of words into groups based on their similarity and provide appropriate category names. The response is in a Python dictionary format as specified in the question.  
- wizardLM-7B.q4_2 (in GPT4All) : 1  
- gpt4all-j-v1.3-groovy (in GPT4All) : 1  
- vicuna-13b-1.1-q4_1 (in GPT4All) : 4  
- gpt4-x-alpaca-13b-ggml-q4_0 (using llama.cpp) : 3  
- koala-13B-4bit-128g.GGML (using llama.cpp) : 1  
- wizard-vicuna-13B.ggml.q4_0 (using llama.cpp) : 4  
- mpt-7b-chat (in GPT4All) : 3  
- stable-vicuna-13B-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 4  
- mpt-7b-instruct : 7  
- wizard-lm-uncensored-13b-GPTQ-4bit-128g (using oobabooga/text-generation-webui) : 5  
- Manticore-13B-GPTQ (using oobabooga/text-generation-webui) : 3  
- manticore_13b_chat_pyg_GPTQ (using oobabooga/text-generation-webui) : 1  
