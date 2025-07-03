# 🧠 BlockoBot — YouTube RAG QA Bot with LangChain, Whisper & LangSmith

A **multimodal AI chatbot** that transforms _Life Noggin_ YouTube videos into interactive knowledge.  
It uses **speech recognition**, **language modeling**, and **retrieval-augmented generation (RAG)** to let users query video content in natural language — either by voice or text.

---

## 🚀 Features

- 🎬 **YouTube Integration** — Downloads and transcribes videos  
- 🗣️ **Speech-to-Text** — Voice input via Whisper  
- 🔎 **Vector Search** — Transcript chunk retrieval via ChromaDB  
- 🤖 **Mistral LLM** — Accurate and efficient responses via Mistral API  
- 🧠 **LangChain Agents** — Tool usage, memory, and multi-step reasoning  
- 🧪 **LangSmith** — Integrated evaluation and interaction logging  
- 🔊 **TTS Output** — Audio responses using Edge TTS  
- 🌍 **Gradio Interface** — Clean, responsive web interface with audio & text modes  

---

## 📚 Business Case

BlockoBot addresses real-world needs in:

- **Accessibility**: Helping hearing-impaired users engage with video content  
- **Searchability**: Instant retrieval of information from video libraries  
- **Education & Training**: Enhances learning by enabling targeted content queries  

---

## 🧩 System Architecture

| Component        | Technology Used                            |
|------------------|---------------------------------------------|
| Speech-to-Text   | OpenAI Whisper (base)                       |
| Embeddings       | `sentence-transformers/all-MiniLM-L6-v2`    |
| Vector DB        | ChromaDB                                    |
| LLM              | Mistral API (`mistral-large-latest`)        |
| Orchestration    | LangChain Agents + Memory + Tools           |
| Evaluation       | LangSmith (tracing & logging)               |
| UI               | Gradio (multimodal support)                 |

---

## 📁 Project Structure

```
LifeNoggingBot/
└── youtube_rag_project/
    ├── audio/                # Downloaded YouTube audio (.mp3)
    ├── transcripts/          # Whisper-generated transcripts (.txt)
    ├── chroma_db/            # Vector store files
    ├── tts/                  # Text-to-speech audio output
picture/
├── blocko.png                # Bot avatar
├── channels4_banner.jpg      # Banner image
main.py                       # Main application file
README.md
```

---

## 🧪 Example Queries

Try asking:

- “What happens to your body in space?”
- “Is AI dangerous?”
- “How much caffeine is safe per day?”

Use the voice interface or type directly into the chatbot.

---

## 📦 Dependencies

```
langchain
langsmith
openai-whisper
edge-tts
mistralai
gradio
pydantic
librosa
yt-dlp
sentence-transformers
chromadb
ffmpeg
nest_asyncio
```

---

## 🙏 Thanks to

**Ironhack AI Bootcamp** for the project inspiration and guidance.

📽️ [View the presentation](https://docs.google.com/presentation/d/1Hb2tPkK2Y1cxz9B5P_u9iU46qbnEx0kF/edit?usp=sharing&ouid=104049074496507203444&rtpof=true&sd=true)