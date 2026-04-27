# nlp-nmt-seq2seq-transformer
# Neural Machine Translation (French → English)
### Seq2Seq with Attention & Transformer Models

This repository contains an implementation of **Neural Machine Translation (NMT)** systems that translate **French sentences into English**, developed as part of the **Natural Language Processing (NLP)** course at the **Faculty of Engineering, Alexandria University**.

Two sequence-to-sequence architectures are implemented **from scratch** and compared:
- **Transformer-based Encoder–Decoder**
- **Seq2Seq model using BiLSTM Encoder, LSTM Decoder, and Additive Attention**

---

## 📌 Project Objectives

- Implement a **Transformer-based NMT model** without relying on PyTorch’s built-in multi-head attention.
- Implement a **Recurrent Seq2Seq NMT model** with additive (Bahdanau) attention.
- Apply **BPE tokenization** for handling rare and out-of-vocabulary words.
- Evaluate both models using the **BLEU score**.
- Visualize **attention weights** to improve interpretability.
- Implement **beam search decoding** for inference.
- Support **checkpoint saving and loading**.

---

## 🏗️ Models Implemented

### 1️⃣ Transformer-Based NMT

**Architecture highlights:**
- Encoder–Decoder Transformer
- Learned positional embeddings
- Multi-head self-attention (implemented manually)
- Causal masking in decoder self-attention
- Residual connections + Layer Normalization
- Weight tying between decoder embeddings and output projection

**Key hyperparameters:**
- Embedding size: 32  
- Number of heads: 4  
- Encoder layers: 3  
- Decoder layers: 3  
- Max sequence length: 32  

---

### 2️⃣ Seq2Seq with BiLSTM + Additive Attention

**Architecture highlights:**
- Bidirectional LSTM encoder
- Unidirectional LSTM decoder
- Additive (Bahdanau) attention mechanism
- Context vector concatenated with decoder input
- Teacher forcing during training

**Key hyperparameters:**
- Embedding size: 256  
- Hidden size: 512  
- Encoder: Bidirectional LSTM  
- Decoder: LSTM  

### 🔗 Collaborators

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/Malak Aboouf">
        <img src="https://github.com/malakaboouf.png" width="100px;" alt="Malak Aboouf"/><br />
        <sub><b>Malak Aboouf</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/reemtest">
        <img src="https://github.com/reemtest.png" width="100px;" alt="reemtest"/><br />
        <sub><b>reemtest</b></sub>
      </a>
    </td>
  </tr>
</table>

