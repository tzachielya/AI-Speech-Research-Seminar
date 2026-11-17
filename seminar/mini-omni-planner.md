# Mini-Omni — Seminar Project Planner (slide transcript)

**Prepared/presented by Tzachi Elya.** This is a text-based transcription of the provided five-slide presentation. The stated month estimates and model-training specifications are a **hypothetical plan/description of the studied approach**, not evidence that I trained Mini-Omni.

## Slide 1 — Topic
**Mini-Omni: Language Models Can Hear, Talk While Thinking in Streaming**  
PLANNER — TZACHI ELYA

## Slide 2 — Method Formulation (approximately 1 month)
- Plan how to build the model
- Read prior research papers
- Design the model structure
- Develop training methods for text and speech together
- Choose tools for speech and text processing

## Slide 3 — Dataset Collection and Preprocessing (approximately 1.5 months)
- Select appropriate sources
- **Text-only:** OpenOrca (2M samples), Wikipedia, C4, books
- **Speech-only:** 8,000 hours (LibriSpeech, VCTK)
- **Text–speech:** 1.5M pairs of synthesized speech and text
- **VoiceAssistant-400K:** Dataset described for speech-model training

## Slide 4 — Implementation and Development (approximately 2 months)
- Write model code, train the model and tune parameters
- Training specified as 40,000 steps with batch size 192
- Train two versions: Basic and Expressive
- Whisper-small used as a speech encoder
- **Stage 1 — Modality Alignment:** link speech and text with adapters
- **Stage 2 — Adaptation Training:** improve joint understanding of text and speech
- **Stage 3 — Multimodal Fine-tuning:** optimize the full model

## Slide 5 — Experiments (approximately 1 month)
- Evaluate speech-to-text accuracy (ASR) against Whisper-small and VITA
- Evaluate question answering for text and speech (TextQA, SpeechQA)
- Evaluate speed and quality changes from Batch Parallel Decoding
- Compare word error rate (WER): **lower is better**.

| Model | test-clean WER | test-other WER | dev-clean WER | dev-other WER |
|---|---:|---:|---:|---:|
| wav2vec2-base | 6.0 | 13.4 | – | – |
| VITA | 8.14 | 18.41 | 7.57 | 16.57 |
| Whisper-small | 3.4 | 7.6 | – | – |
| Mini-Omni | 4.5 | 9.7 | 4.6 | 9.2 |

As described in the slide, Mini-Omni outperforms VITA on the two comparable test sets, but trails Whisper-small on those sets.

---

**Note:** These results are reproduced from the table shown in the provided slide deck. They are research comparison figures, *not experiments conducted by the presenter*. The original PowerPoint contains the formatted slide design and an image of the table; this text transcript provides its contents.
