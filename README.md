# Microsoft AI-900 Master Notes

> A GitHub-ready study guide for **Microsoft Azure AI Fundamentals (AI-900)**.  
> Focus: exam definitions, scenario-based decision rules, Azure AI services, Microsoft Foundry, responsible AI, machine learning, NLP, Speech, Vision, OCR, Document Intelligence, and AI Search.

---

# AI-900 Master Notes

📁 **Full Study Materials (Google Drive):**  
👉 https://drive.google.com/drive/folders/13i54qqovtSzoDV8qZXZL5MATA8wpN5wN?usp=sharing

---

## Table of Contents

1. [AI Fundamentals](#1-ai-fundamentals)
2. [Machine Learning Basics](#2-machine-learning-basics)
3. [Generative AI](#3-generative-ai)
4. [Microsoft Foundry](#4-microsoft-foundry)
5. [Natural Language Processing](#5-natural-language-processing)
6. [Azure Speech](#6-azure-speech)
7. [Computer Vision](#7-computer-vision)
8. [Information Extraction, OCR, and Document Intelligence](#8-information-extraction-ocr-and-document-intelligence)
9. [Azure AI Search and Knowledge Mining](#9-azure-ai-search-and-knowledge-mining)
10. [Responsible AI](#10-responsible-ai)
11. [Azure Basics for AI-900](#11-azure-basics-for-ai-900)
12. [Cloud Service Models](#12-cloud-service-models)
13. [Exam Traps and Decision Rules](#13-exam-traps-and-decision-rules)
14. [Final One-Page Cheat Sheet](#14-final-one-page-cheat-sheet)

---

# 1. AI Fundamentals

## What is Artificial Intelligence?

**Artificial Intelligence (AI)** is the broad field of creating systems that can perform tasks that normally require human intelligence.

Examples of AI tasks:

- Understanding language
- Recognizing images
- Reasoning
- Solving problems
- Making predictions
- Responding to users
- Automating decisions or workflows

### Exam Focus

AI is the **broad goal**: making systems act intelligently.

---

## AI vs Machine Learning vs Deep Learning vs Generative AI

| Concept | Meaning | Exam Keyword |
|---|---|---|
| **AI** | Broad field of human-like intelligence | Intelligent systems |
| **Machine Learning** | Systems learn patterns from data | Learns from data |
| **Deep Learning** | ML using neural networks with many layers | Neural networks |
| **Generative AI** | Creates new content | Text, image, code, audio generation |

### Very Important Sentence

> **AI is the overall goal. Machine Learning is a data-driven method used to achieve AI.**

---

# 2. Machine Learning Basics

## What is Machine Learning?

**Machine Learning (ML)** is a method of building AI systems where the system learns patterns from data instead of being programmed with fixed rules.

A simple ML model can be described as:

```text
x → f(x) → ŷ
```

| Symbol | Meaning |
|---|---|
| `x` | Input features |
| `f(x)` | Model function |
| `ŷ` | Prediction |
| `y` | True label/output |

---

## Types of Machine Learning

### 1. Supervised Learning

Supervised learning uses **labeled data**.

The training data includes both:

- Input features
- Correct answers/labels

Examples:

| Task | Meaning | Example |
|---|---|---|
| **Regression** | Predicts a number | Predict house price |
| **Classification** | Predicts a category | Spam or not spam |

### 2. Unsupervised Learning

Unsupervised learning uses **unlabeled data**.

The model finds patterns or groups by itself.

| Task | Meaning | Example |
|---|---|---|
| **Clustering** | Groups similar data | Customer segmentation |

### 3. Deep Learning

Deep learning is a type of machine learning that uses **neural networks with many layers**.

Common uses:

- Image recognition
- Speech recognition
- Speech synthesis
- Natural language processing
- Generative AI

---

## Regression vs Classification vs Clustering

| Problem Type | Correct ML Task |
|---|---|
| Predict a price | Regression |
| Predict yes/no | Binary classification |
| Predict one of many categories | Multiclass classification |
| Group similar customers | Clustering |

### Memory Rule

- **Regression = number**
- **Classification = category**
- **Clustering = grouping**

---

## Machine Learning Metrics

### Regression Metrics

| Metric | Meaning |
|---|---|
| **MAE** | Mean Absolute Error; average prediction error |
| **RMSE** | Root Mean Squared Error; penalizes large errors more heavily |
| **R²** | Shows how well the model explains variation; closer to 1 is better |

### Classification Metrics

| Metric | Meaning |
|---|---|
| **Accuracy** | Overall percentage of correct predictions |
| **Precision** | Of predicted positives, how many were actually positive |
| **Recall** | Of actual positives, how many were found |
| **F1-score** | Balance between precision and recall |

---

## ML Process

A common ML process is:

1. Train
2. Validate
3. Evaluate
4. Improve
5. Retrain when needed

Machine learning is usually **iterative**, meaning the model is improved over time.

---

## ML Lifecycle

Memory phrase:

```text
D G P T I M
```

| Step | Meaning |
|---|---|
| **Define** | Define the business problem |
| **Get data** | Collect relevant data |
| **Prepare** | Clean and transform data |
| **Train** | Train the model |
| **Integrate** | Deploy or connect the model to an app |
| **Monitor** | Track performance and improve over time |

---

## Data Types

| Data Type | Example |
|---|---|
| **Structured** | Tables, databases, SQL rows |
| **Semi-structured** | JSON, XML |
| **Unstructured** | Images, audio, text, videos, PDFs |

---

## ETL Pipeline

ETL means:

```text
Extract → Transform → Load
```

| Step | Meaning |
|---|---|
| **Extract** | Get data from sources |
| **Transform** | Clean or prepare data |
| **Load** | Store data in the target system |

---

## Azure ML Services

| Service | Best Use |
|---|---|
| **Azure Machine Learning** | Build, train, evaluate, deploy ML models |
| **Databricks** | Big data analytics and ML workloads |
| **Microsoft Fabric** | Data analytics and reporting |
| **Microsoft Foundry** | Build AI apps using models, tools, agents, and prebuilt services |

---

## Azure Machine Learning Features

Azure Machine Learning can be used to:

- Import and explore data
- Create compute resources
- Run notebooks
- Use visual tools
- Use Automated ML
- Train models
- Evaluate models
- Deploy models
- Monitor model performance

### AutoML

**Automated Machine Learning (AutoML)** automatically tries multiple algorithms and selects a strong model.

Exam focus:

> AutoML helps automate **model training and selection**. It is not mainly a deployment tool.

---

## Real-Time vs Batch Inferencing

| Type | Meaning | Best For |
|---|---|---|
| **Real-time inference** | Immediate prediction through an API endpoint | Live app, chatbot, instant decision |
| **Batch inference** | Processes many records on a schedule | Large datasets, reports, offline scoring |

### Exam Rule

Choose based on **speed requirement**, not only data frequency.

---

# 3. Generative AI

## What is Generative AI?

**Generative AI** creates new content based on patterns learned from training data.

It can generate:

- Text
- Images
- Audio
- Video
- Code

### Exam Focus

Generative AI is about **creating new content**, not only analyzing existing data.

---

## Large Language Models

A **Large Language Model (LLM)** is trained on huge amounts of text and can generate human-like language.

Key idea:

> An LLM predicts the next token based on context.

---

## Tokens and Tokenization

**Tokenization** means breaking text into smaller pieces called tokens.

Tokens can be:

- Words
- Parts of words
- Symbols
- Punctuation

Example:

```text
Machine learning is useful.
```

Could become:

```text
[Machine] [learning] [is] [useful] [.]
```

---

## Embeddings

**Embeddings** convert words, sentences, documents, or tokens into numerical vectors.

Purpose:

- Capture meaning
- Compare similarity
- Support search and retrieval
- Power RAG systems

### Exam Focus

Embeddings represent **meaning as numbers**.

---

## Attention and Transformers

**Attention** helps a model focus on the most important words or tokens in context.

**Transformers** are important because they use attention mechanisms to understand relationships in sequences.

### Exam Focus

Transformers are critical for LLMs because they enable attention and help models handle long-range dependencies in text.

---

## Prompts

A **prompt** is the input given to a generative AI model.

### System Prompt

A system prompt controls the model's behavior, rules, tone, and boundaries.

Example:

```text
You are a helpful assistant. Answer clearly and professionally.
```

### User Prompt

A user prompt is the actual question or request.

Example:

```text
Explain machine learning in simple words.
```

---

## RAG: Retrieval-Augmented Generation

**RAG** means combining an LLM with external data.

Simple formula:

```text
RAG = Retrieve relevant information + Generate answer
```

RAG helps the model answer using company documents, search indexes, or knowledge bases.

### Very Important Exam Rule

> RAG does **not** train the model. RAG adds external context at response time.

---

## Fine-Tuning vs Grounding vs RAG

| Method | Meaning | Exam Keyword |
|---|---|---|
| **Grounding** | Connect the model to reliable data | Use real data/context |
| **RAG** | Retrieve external data before generating | External context, not training |
| **Fine-tuning** | Train/customize model weights using data | Training/customization |

---

## AI Agents

An **AI agent** can reason, use tools, and take actions.

Formula:

```text
Agent = LLM + Instructions + Tools
```

Examples of agent tools:

- Knowledge tools: search documents or databases
- Action tools: call APIs, create tickets, send messages, trigger workflows

### Assistant vs Agent

| Type | Main Role |
|---|---|
| **Assistant** | Answers questions |
| **Agent** | Answers and acts using tools |

---

# 4. Microsoft Foundry

## What is Microsoft Foundry?

**Microsoft Foundry** is a unified enterprise AI platform for building, testing, deploying, monitoring, and governing AI applications and agents.

It brings together:

- Models
- Agents
- Tools
- Playgrounds
- Evaluation
- Observability
- Governance
- Security

### Simple Definition

> Foundry is an all-in-one platform for enterprise AI development.

---

## Foundry Structure

| Component | Meaning |
|---|---|
| **Hub** | Main environment that can connect shared resources and capabilities |
| **Project** | Main workspace for building AI apps and agents |

### Exam Focus

The **project** is usually the main workspace where you build and manage AI applications.

---

## Foundry Components

| Component | Purpose |
|---|---|
| **Model Catalog** | Find, compare, test, and deploy models |
| **Playground** | Test models without coding |
| **Agent Service** | Build agents and workflows |
| **Foundry Tools** | Use prebuilt AI services like Vision, Speech, Language, Search, and Document Intelligence |
| **Observability** | Monitor quality, performance, usage, and safety |
| **Governance** | Manage compliance, policies, identity, security, and responsible AI controls |

---

## Foundry Models

Foundry Models provide access to a model catalog.

You can:

- Browse models
- Compare models
- Test models in playgrounds
- Deploy models
- Customize models
- Manage versions

Examples of foundation models:

- Azure OpenAI models
- GPT models
- Llama
- Mistral
- Cohere
- Anthropic models

---

## Foundation Models

A **foundation model** is a pretrained model that can be used for many tasks.

Benefits:

- Ready to use
- Saves time
- Avoids training from scratch
- Can sometimes be customized or fine-tuned

---

## Observability in Foundry

Observability means monitoring and evaluating AI systems after and during development.

Main evaluation areas:

| Area | Meaning |
|---|---|
| **Performance and quality** | Accuracy, relevance, groundedness, fluency, coherence |
| **Risk and safety** | Harmful content, unsafe outputs, policy risks |
| **Custom evaluators** | Business-specific or industry-specific metrics |

### Common Evaluators

| Evaluator | Meaning |
|---|---|
| **Groundedness** | Is the answer supported by retrieved/context data? |
| **Relevance** | Does the answer match the question? |
| **Fluency** | Is the language readable and natural? |
| **Coherence** | Is the answer logical and well-structured? |
| **Safety** | Does the answer avoid harmful content? |

---

# 5. Natural Language Processing

## What is NLP?

**Natural Language Processing (NLP)** is AI for understanding, analyzing, and processing human language.

Simple difference:

| Concept | Meaning |
|---|---|
| **NLP** | Understands and analyzes language |
| **Generative AI** | Creates new content or language |

---

## Core NLP Tasks

| Task | Meaning | Example |
|---|---|---|
| **Language detection** | Detect language of text | “Bonjour” → French |
| **Text classification** | Assign text to categories | Complaint, feedback, question |
| **Sentiment analysis** | Detect positive, negative, or neutral sentiment | Product review analysis |
| **Key phrase extraction** | Find important words/phrases | “battery life”, “camera quality” |
| **Named Entity Recognition** | Detect people, places, organizations, products | Microsoft, Canada |
| **PII detection** | Detect private/sensitive personal information | Email, phone number, address |
| **Summarization** | Shorten long text while keeping main points | Meeting summary |
| **Translation** | Convert text from one language to another | English → French |

---

## NLP Preprocessing

| Technique | Meaning |
|---|---|
| **Normalization** | Lowercase text, remove punctuation, standardize text |
| **Stop word removal** | Remove common words like “the”, “a”, “is” |
| **N-grams** | Groups of words such as bigrams or trigrams |
| **Stemming** | Cut word endings; less accurate |
| **Lemmatization** | Convert word to dictionary/base form; more accurate |
| **POS tagging** | Identify grammar roles like noun, verb, adjective |

---

## Statistical NLP Methods

| Method | Meaning | Exam Keyword |
|---|---|---|
| **Frequency** | Count word occurrences | Topic from repeated words |
| **Bag of Words** | Convert text to word-count vectors | Ignores word order |
| **TF-IDF** | Measures word importance based on frequency and rarity | Rare across documents = important |
| **TextRank** | Graph-based summarization | Extract important sentences |

### TF-IDF Exam Rule

A word has a high TF-IDF score when it is:

- Frequent in one document
- Rare across many documents

Common words usually get a low score.

---

## Semantic NLP Methods

| Method | Meaning |
|---|---|
| **Embeddings** | Convert text into vectors that capture meaning |
| **Cosine similarity** | Measures similarity between vectors |
| **Contextual models** | Understand word meaning based on surrounding context |

### Cosine Similarity

| Score | Meaning |
|---|---|
| Close to 1 | Very similar |
| Close to 0 | Not very similar |

---

## Azure AI Language

**Azure AI Language** is the main Azure service for NLP features.

It supports:

- Language detection
- Sentiment analysis
- Key phrase extraction
- Named Entity Recognition
- Entity linking
- PII detection and redaction
- Summarization
- Conversational Language Understanding
- Question answering

---

## NER vs Entity Linking

| Feature | Meaning |
|---|---|
| **NER** | Finds entities in text |
| **Entity linking** | Connects detected entities to known real-world references |

Example:

```text
Microsoft released a new AI tool.
```

- NER detects: `Microsoft`
- Entity linking connects it to the actual company Microsoft

---

## Question Answering vs CLU

| Feature | Best For | Example |
|---|---|---|
| **Question Answering** | Answering questions from a knowledge base | FAQ chatbot |
| **Conversational Language Understanding (CLU)** | Detecting user intent and entities | “Book a flight to Toronto” |

### Exam Rule

- **QA = answer questions**
- **CLU = understand intent + entities for actions**

---

## Azure Translator

**Azure Translator** uses Neural Machine Translation (NMT).

Important points:

- Context-aware translation
- Not simple word-by-word translation
- Supports text translation
- Supports document translation
- Supports custom translation
- Can translate one source language into multiple target languages

---

# 6. Azure Speech

## Core Speech Concepts

| Concept | Direction | Meaning |
|---|---|---|
| **Speech recognition / ASR** | Audio → Text | Transcribe speech |
| **Speech synthesis / TTS** | Text → Audio | Generate spoken audio |
| **Speech translation** | Speech → Text → Translation | Translate spoken language |

### Exam Memory

- **Speech-to-text = recognition**
- **Text-to-speech = synthesis**

---

## Azure Speech Service

Azure Speech includes:

- Speech-to-text
- Text-to-speech
- Speech translation

It can be used through:

- REST API
- SDK
- Studio/playground interfaces
- CLI

---

## Speech Recognition Pipeline

Memory order:

```text
Audio Capture → Preprocessing → Acoustic Model → Language Model → Decoding → Post-processing
```

| Step | Meaning |
|---|---|
| **Audio capture** | Capture the spoken audio |
| **Preprocessing** | Clean or prepare audio features |
| **Acoustic model** | Maps audio signals to phonemes/sounds |
| **Language model** | Predicts likely words and phrases |
| **Decoding** | Chooses the most likely transcription |
| **Post-processing** | Adds punctuation, formatting, corrections |

---

## Speech Synthesis Pipeline

```text
Text Normalization → Linguistic Analysis → Prosody → Audio Generation
```

| Step | Meaning |
|---|---|
| **Text normalization** | Prepare written text |
| **Linguistic analysis** | Analyze pronunciation and structure |
| **G2P** | Grapheme-to-phoneme conversion; letters to sounds |
| **Prosody** | Pitch, rhythm, tone, stress |
| **Vocoder** | Generates audio waveform |

### Exam Focus

**Prosody** makes generated speech sound natural.

---

## Real-Time vs Batch Speech

| Type | Best For |
|---|---|
| **Real-time speech** | Live transcription or live voice assistant |
| **Batch speech** | Stored audio files, asynchronous processing |

---

## Speech Use Cases

- Voice assistants
- Meeting transcription
- Call center analytics
- Captions
- Accessibility tools
- Reading emails aloud
- Speech translation apps

---

# 7. Computer Vision

## What is Computer Vision?

**Computer Vision** is AI that analyzes visual input such as:

- Images
- Videos
- Camera feeds
- Scanned documents

Images are made of pixels, and pixels are represented by numbers.

---

## Main Vision Tasks

| Task | Output | Exam Keyword |
|---|---|---|
| **Image classification** | One or more labels for the whole image | “What is this image?” |
| **Object detection** | Objects + bounding boxes | “Where are the objects?” |
| **Semantic segmentation** | Pixel-level object regions | “Exact shape / exact pixels” |
| **Captioning** | Sentence describing image | “Describe the image” |
| **Tagging** | Keywords | Search/index images |
| **OCR** | Text from image | Read text |

---

## Classification vs Detection vs Segmentation

| Task | What it Does | Example |
|---|---|---|
| **Classification** | Labels the whole image | Image → “dog” |
| **Object detection** | Finds objects and locations | Dog + bounding box |
| **Segmentation** | Finds exact pixels for each object | Exact dog shape highlighted |

### Exam Memory

- Classification = what
- Detection = what + where
- Segmentation = exact pixels

---

## CNN vs Vision Transformer

| Model | How it Works | Memory Rule |
|---|---|---|
| **CNN** | Uses filters/convolutions to extract features | CNN = filters |
| **Vision Transformer (ViT)** | Uses patches and attention | ViT = attention |

---

## Image Generation with Diffusion

Diffusion models generate images by starting with noise and removing noise step by step until an image matches the prompt.

Memory rule:

```text
Noise → Image
```

---

## Azure AI Vision

Azure AI Vision can support:

- Image analysis
- Captions
- Tags
- Object detection
- OCR

---

## Face Service

Face-related capabilities can include:

| Feature | Meaning |
|---|---|
| **Face detection** | Finds where faces are in an image |
| **Face recognition** | Identifies who a person is |
| **Face attributes** | Detects attributes like glasses, blur, mask |
| **Liveness detection** | Helps determine if a face is from a live person |

### Exam Note

Face identification, verification, and liveness detection are more sensitive and may have restricted access depending on use case and policy.

---

# 8. Information Extraction, OCR, and Document Intelligence

## Core Flow

```text
Image / Document → OCR → Text → Field Extraction → Structured Data → System
```

---

## OCR

**OCR (Optical Character Recognition)** extracts text from images, PDFs, scans, and screenshots.

OCR can identify:

- Where text appears
- What the text says

### Exam Focus

> OCR reads text, but OCR alone does not fully understand document meaning.

---

## Field Extraction

Field extraction maps text to meaningful structured fields.

Example from an invoice:

| Text | Structured Field |
|---|---|
| `INV-1234` | Invoice number |
| `$250.00` | Total amount |
| `May 4, 2026` | Invoice date |

---

## Azure Document Intelligence

**Azure Document Intelligence** is used to extract structured information from documents such as:

- Receipts
- Invoices
- Forms
- Contracts
- IDs
- Business documents

It supports:

- Prebuilt models
- Custom models
- Field extraction
- Layout extraction

### Exam Rule

For invoices, receipts, forms, and structured documents, choose **Document Intelligence**.

---

## Azure Content Understanding

**Azure Content Understanding** can process multiple content types, including:

- Documents
- Images
- Audio
- Video

It can be useful for multimodal extraction, schema-based extraction, and summarization.

### Exam Rule

For multimodal content such as audio + video + documents, choose **Content Understanding**.

---

## Service Selection Table

| Scenario | Best Azure Service |
|---|---|
| Extract fields from invoice | Document Intelligence |
| Extract total amount from receipt | Document Intelligence |
| Read text from an image | OCR / Azure Vision |
| Analyze objects in a photo | Azure AI Vision |
| Summarize mixed audio/video/document content | Content Understanding |
| Make documents searchable | Azure AI Search |

---

# 9. Azure AI Search and Knowledge Mining

## What is Azure AI Search?

**Azure AI Search** is a cloud service for indexing and searching data.

It can be used to build:

- Search experiences
- Knowledge mining solutions
- RAG retrieval systems
- Enterprise document search

---

## Key AI Search Components

| Component | Meaning |
|---|---|
| **Indexer** | Pipeline that pulls data from a source and processes it |
| **Index** | Searchable structure that stores searchable fields |
| **AI skills** | Enrichment steps that extract insights from content |
| **Data source** | Original data location, such as Blob Storage or a database |

---

## Knowledge Mining Flow

```text
Data Source → Indexer → AI Skills → Index → Search Application
```

Examples of AI enrichment:

- OCR text extraction
- Key phrase extraction
- Entity recognition
- Language detection
- Image analysis
- Document cracking

---

## Exam Focus

If the scenario says:

- “Make documents searchable”
- “Create a search index”
- “Use AI skills to enrich documents”
- “Knowledge mining”

The answer is usually **Azure AI Search**.

---

# 10. Responsible AI

Responsible AI means building and using AI systems in a way that is ethical, safe, fair, secure, and accountable.

## The 6 Responsible AI Principles

| Principle | Meaning | Exam Keyword |
|---|---|---|
| **Fairness** | AI should not discriminate | Bias, discrimination |
| **Reliability and Safety** | AI should work safely and avoid harm | Safety, confidence threshold |
| **Privacy and Security** | Protect data and private information | PII, secure data |
| **Inclusiveness** | AI should work for all people | Accessibility, disability support |
| **Transparency** | Users should know AI is used and understand limitations | Disclosure, explainability |
| **Accountability** | Humans/organizations are responsible for AI systems | Governance, ownership |

---

## Responsible AI Scenario Matching

| Scenario | Principle |
|---|---|
| AI should not discriminate against groups | Fairness |
| Robot should act only with high confidence | Reliability and Safety |
| Temporary face images should be deleted | Privacy and Security |
| App should support users with disabilities | Inclusiveness |
| Bank explains AI is used in loan decisions | Transparency |
| Company creates AI governance policies | Accountability |

---

# 11. Azure Basics for AI-900

## What is Azure?

**Microsoft Azure** is Microsoft’s cloud computing platform for building, deploying, and managing applications and services through Microsoft-managed data centers.

Azure provides:

- Compute
- Storage
- Networking
- Application services
- AI services
- Security and identity tools

---

## Azure Core Capabilities

| Capability | Meaning | Examples |
|---|---|---|
| **Compute** | Runs applications/workloads | Virtual Machines, Azure Functions, Containers |
| **Storage** | Stores files and data | Blob Storage, Azure Files, Data Lake |
| **Networking** | Connects and secures resources | Virtual Network, Load Balancer |
| **Application services** | Build and host apps | Web Apps, APIs, mobile backends |

---

## Azure Resource Organization

Azure hierarchy:

```text
Tenant → Subscription → Resource Group → Resource
```

| Level | Meaning | Main Role |
|---|---|---|
| **Tenant** | Organization identity | Users, authentication, Microsoft Entra ID |
| **Subscription** | Billing and access boundary | Payment, limits, service access |
| **Resource Group** | Logical container | Organize related resources |
| **Resource** | Actual Azure service | VM, database, AI service |

### Common Exam Traps

| Wrong Idea | Correct Idea |
|---|---|
| Resource groups handle billing | Subscriptions handle billing |
| Resources contain resource groups | Resource groups contain resources |
| Tenant is mainly for compute/storage | Tenant is mainly for identity and access management |

---

## API Access: Key and Endpoint

To call many Azure AI services from an app, you need:

| Item | Meaning |
|---|---|
| **Endpoint** | URL/address of the service |
| **Key** | Secret credential used to authenticate |
| **Authentication header** | Sends the key with the request |

### Exam Focus

Key + endpoint are commonly required to call Azure AI APIs securely.

---

# 12. Cloud Service Models

## IaaS, PaaS, SaaS

| Model | Meaning | User Responsibility | Example |
|---|---|---|---|
| **IaaS** | Infrastructure as a Service | High | Virtual Machine |
| **PaaS** | Platform as a Service | Medium | Azure App Service, Azure SQL, Foundry services |
| **SaaS** | Software as a Service | Low | Microsoft 365, Gmail |

---

## Memory Rule

| Model | Simple Analogy |
|---|---|
| **IaaS** | Rent an empty apartment; you manage more |
| **PaaS** | Rent a ready kitchen; you focus on cooking/building |
| **SaaS** | Order food; you just use the service |

---

# 13. Exam Traps and Decision Rules

## High-Yield Traps

| Trap | Correct Answer |
|---|---|
| Regression vs classification | Number vs category |
| Supervised vs unsupervised | Labels vs no labels |
| AutoML | Automates model training/selection |
| Real-time vs batch | Choose based on speed requirement |
| Azure ML vs Foundry | Azure ML builds custom ML; Foundry builds AI apps with models/tools/agents |
| RAG vs fine-tuning | RAG adds context; fine-tuning trains/customizes model |
| OCR vs Document Intelligence | OCR reads text; Document Intelligence extracts structured fields |
| Object detection vs segmentation | Detection uses boxes; segmentation uses pixels |
| QA vs CLU | QA answers; CLU detects intent/entities |
| Speech recognition vs synthesis | Audio→text vs text→audio |
| Subscription vs resource group | Billing/access vs organization container |

---

## Scenario Triggers

| If the question says... | Choose... |
|---|---|
| “Predict a numeric value” | Regression |
| “Predict a category” | Classification |
| “Group similar data without labels” | Clustering |
| “Convert speech to text” | Speech recognition |
| “Convert text to speech” | Speech synthesis |
| “Find objects and draw boxes” | Object detection |
| “Find exact pixels of an object” | Semantic segmentation |
| “Extract text from image” | OCR |
| “Extract fields from invoice/receipt/form” | Document Intelligence |
| “Make documents searchable” | Azure AI Search |
| “Detect private information” | PII detection |
| “Avoid discrimination” | Fairness |
| “Protect personal data” | Privacy and Security |
| “Tell users AI is being used” | Transparency |
| “Human responsibility/governance” | Accountability |
| “Intent and entities” | CLU |
| “FAQ chatbot / knowledge base answers” | Question Answering |
| “Use external data without training model” | RAG |
| “Train/customize model weights” | Fine-tuning |
| “Monitor groundedness/relevance/safety” | Observability |

---

# 14. Final One-Page Cheat Sheet

## AI Concepts

```text
AI = human-like intelligence
ML = learns from data
Deep Learning = neural networks
Generative AI = creates content
```

## ML

```text
Regression = number
Classification = category
Clustering = grouping
Supervised = labeled data
Unsupervised = unlabeled data
AutoML = automatic training/selection
Endpoint = API access to deployed model
```

## Generative AI

```text
LLM = predicts next token
Prompt = input
System prompt = rules/behavior
User prompt = question/request
Embeddings = meaning as vectors
RAG = external context, not training
Fine-tuning = training/customization
Agent = LLM + instructions + tools
```

## Responsible AI

```text
Fairness = avoid bias
Reliability/Safety = avoid harm
Privacy/Security = protect data
Inclusiveness = accessibility
Transparency = disclose/explain AI use
Accountability = humans/orgs responsible
```

## NLP

```text
Azure AI Language = main NLP service
NER = find entities
Entity linking = connect entity to real-world reference
PII = detect sensitive data
Sentiment = positive/neutral/negative
Key phrases = main ideas
QA = answers
CLU = intent + entities
Translator = Neural Machine Translation
```

## Speech

```text
Speech recognition = speech → text
Speech synthesis = text → speech
Speech translation = speech → text → translation
Prosody = pitch/tone/rhythm for natural voice
Real-time = live
Batch = stored audio
```

## Vision

```text
Classification = image label
Detection = objects + bounding boxes
Segmentation = pixel-level exact shape
Caption = sentence description
Tagging = keywords
OCR = read text
CNN = filters
ViT = attention
Diffusion = noise → image
```

## Documents and Search

```text
OCR = image/document → text
Field extraction = text → structured data
Document Intelligence = forms, invoices, receipts
Content Understanding = multimodal content
AI Search = searchable index + knowledge mining
Indexer = pipeline
Index = searchable data
AI Skills = enrichment
```

## Azure

```text
Tenant = identity
Subscription = billing/access
Resource Group = related resources
Resource = actual service
Key = secret credential
Endpoint = service URL
```

## Cloud Models

```text
IaaS = manage more
PaaS = build apps, less infrastructure
SaaS = ready-to-use software
```

---

# Recommended GitHub README Structure

If you want to use these notes as a GitHub repository README, a good repo structure would be:

```text
ai-900-study-notes/
├── README.md
├── cheatsheets/
│   ├── responsible-ai.md
│   ├── machine-learning.md
│   ├── generative-ai.md
│   ├── nlp.md
│   ├── speech.md
│   ├── vision.md
│   └── document-intelligence-search.md
└── practice-questions/
    └── ai-900-practice-questions.md
```

Suggested README title:

```markdown
# Microsoft AI-900 Study Notes

A complete exam-focused study guide for Microsoft Azure AI Fundamentals.
```

---

## Final Exam Advice

AI-900 questions are often scenario-based. Do not only memorize definitions. Focus on matching the scenario to the correct service, concept, workload, or Responsible AI principle.

The most important exam skill is recognizing keywords:

- **Number prediction** → Regression
- **Category prediction** → Classification
- **Grouping without labels** → Clustering
- **Speech to text** → Speech recognition
- **Text to speech** → Speech synthesis
- **Bounding boxes** → Object detection
- **Exact pixels** → Segmentation
- **Invoices/receipts/forms** → Document Intelligence
- **Searchable documents** → Azure AI Search
- **Bias/discrimination** → Fairness
- **External data without training** → RAG
- **Intent + entities** → CLU
