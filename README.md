### 🧠 Fine-tuning HerBERT on Pan Tadeusz

`Jagiellonian University – Final project nr. 4 for the course Machine Learning 2021`

---

### 📚 Project Description

This project involves fine-tuning the HerBERT model — a transformer-based language model pretrained on a large Polish corpus. The model, originally an encoder-only architecture (RoBERTa), was adapted for causal language modeling using the RobertaForCausalLM class with is_decoder=True.

However, to better align with the causal language modeling task, I also fine-tuned a GPT-2-like decoder model — papuGaPT2 — which was specifically pretrained for autoregressive text generation on a large Polish corpus.

The training was performed on Pan Tadeusz, a classic Polish epic poem by Adam Mickiewicz. The task was to train both models to generate coherent text in the style of the poem. After each training epoch, sample text was generated from the prompt Jam jest Jacek, and perplexity was recorded on the training and validation sets.

---

### 🧠 Models Used

    allegro/herbert-klej-cased-v1

    flax-community/papuGaPT2

---

### 📂 Dataset

The dataset consists of the full text of Pan Tadeusz, split into:

    pan_tadeusz_1_10.txt – training (Books 1–10)

    pan_tadeusz_11.txt – validation (Book 11)

    pan_tadeusz_12.txt – test (Book 12)

---

### 🧾 References

   - 🔗 [UJ Machine Learning Course 2021/2022](https://sites.google.com/view/uczeniemaszynowe2021/home) – Course homepage  
  - 📄 [Final Project Description – Project 4](https://docs.google.com/document/d/1VK3003LuW5TMllkJ0wWHEMG8PObgxropPYtnIvr6nUo/edit?tab=t.0) – Official instructions for the assignment
