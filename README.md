# AI Speech & Language Models — Academic Seminar

**Research presentation and critical paper review by Tzachi Elya**  
**Topic:** [Mini-Omni: Language Models Can Hear, Talk While Thinking in Streaming](https://arxiv.org/abs/2408.16725)

This repository presents a university seminar assignment about **real-time speech-to-speech generative AI**. It contains a five-slide research-based project planner and a written critical review of the Mini-Omni paper.

> **Academic scope:** This is a presentation, planning exercise, and literature review — **not an implemented, trained, or deployed AI model**. Architecture descriptions, training steps, data sizes, and experimental results are discussed as part of the reviewed research/proposed implementation plan; they are not claimed as my own experimental results.

## Seminar materials

- [Presentation — annotated slide transcript](seminar/mini-omni-planner.md): key concepts, proposed research/engineering phases, dataset requirements, training strategy, and evaluation approaches.
- [Critical review](seminar/mini-omni-paper-review.md): research summary, strengths, limitations, and questions for discussion.

The original submitted source files were `planner - tzachi .pptx` and `review.pdf`. The linked repository files are **readable Markdown transcriptions**, not the original binary PPTX or PDF attachments. A comparison table appearing as an image in the slide deck is reproduced numerically in the transcript.

## Research focus

**Mini-Omni** explores a language model that understands and generates text and audio in streaming, reducing conversational latency. The seminar materials cover:

- **System design:** speech and text modality alignment, speech encoding with Whisper-small, and multimodal training.
- **Data preparation:** text-only, speech-only and text–speech datasets, plus the paper's VoiceAssistant-400K contribution.
- **Model evaluation:** ASR quality (Word Error Rate), text/speech question answering, and streaming-speed considerations.
- **Critical review:** limited comparisons to other models, evaluation under noisy/real-world conditions, diverse accents/languages and hardware/training cost transparency.

## What I did

1. Studied and presented the Mini-Omni research in an academic seminar setting.
2. Prepared a structured presentation outlining a possible project plan for reproducing the research (methodology, data, development phases and evaluation).
3. Wrote a critical review of the paper's soundness, clarity, contribution and limitations.
4. Formulated discussion questions for evaluating the model's data and outcomes.

## Relevance

This seminar demonstrates **technical research literacy**, **structured thinking**, **critical evaluation of AI claims**, and **communication of complex technology**. The technical design and evaluation were researched/presented, not independently implemented.

## Source

*Mini-Omni: Language Models Can Hear, Talk While Thinking in Streaming*, research paper discussed in the academic seminar.
