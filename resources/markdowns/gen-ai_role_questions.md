# Gen-AI related Topics

<details>
  <summary>FAQs</summary>

<!-- ################################################### The FAQ list starts here ################################################### -->

  <details>
    <summary>What is RAG?</summary>
    <p>
    Retrieval-Augmented Generation (RAG) is a hybrid architecture that combines retrieval-based search with large language models (LLMs) to enhance factuality, scalability, and adaptability. Traditional LLMs rely solely on their training data, making them prone to factual errors or outdated knowledge. In RAG, when a user submits a query, a retriever module (such as a dense vector search against a vector database) identifies the most relevant documents or context snippets from an external knowledge store or corpus. These retrieved pieces are fed, along with the user’s query, into a generative model (such as GPT or Llama). The generation process then conditions on this fresh information, allowing the LLM to produce answers that are not only contextual but also grounded in the latest or domain-specific data.

    RAG offers several technical advantages. It reduces hallucination by anchoring outputs to retrievable facts, supports handling proprietary or changing corpora without retraining, and is highly modular—retrievers and generators can be independently optimized and updated. RAG pipelines typically include pre-processing (embedding and indexing data), retrieval (using approximate nearest neighbor or BM25 algorithms), fusion (combining multiple retrieved snippets), and generation. Evaluation metrics include factual consistency, retrieval precision, and relevance. RAG is central in enterprise knowledge assistants, document Q&A, and scenarios demanding transparency and up-to-date completions.
    </p>
  </details>

  <details>
    <summary>How do you evaluate GenAI outputs?</summary>
    <p>
    Evaluating GenAI outputs involves multifaceted strategies, blending automatic and human approaches to cover the complexity of generative responses. Automated metrics, such as BLEU, ROUGE, and METEOR, provide quantitative assessments of overlap with reference texts, but are limited in capturing contextual relevance, creativity, or logical reasoning. More sophisticated metrics—like BERTScore or COMET—leverage transformer models for semantic similarity evaluation. However, generative tasks often require qualitative judgments, leading to the use of human evaluation along dimensions such as accuracy, relevance, coherence, fluency, informativeness, user satisfaction, and avoidance of harmful content.

    For domain-specific applications, you would design task-based and user-centric metrics—for instance, correctness in legal summaries or safety in medical advice. Adversarial testing (feeding edge cases and outliers to the model) uncovers robustness and bias. Another emerging technique is LLM-as-a-judge, using a strong LLM to grade outputs, which can scale evaluations but risks propagating model-specific biases and flaws.

    Long-term monitoring involves capturing and analyzing user feedback, complaints, and session ratings for iterative improvement. For chatbots, dialogue flow analysis, task-completion rates, and fallback rates (how often a deterministic fallback is triggered) are tracked. End-to-end evaluation pipelines combine these methods, providing a holistic picture and enabling continuous retraining and deployment cycles to maintain high output quality.
    </p>
  </details>

  <details>
    <summary>A chatbot shows gender bias, e.g., HR jobs to women and Engineering jobs to men. How do you detect and fix this?</summary>
    <p>
    Detecting and remediating gender bias in chatbots requires a combination of systematic evaluation and targeted reengineering. Detection starts with input audits: prompt the bot with gender-neutral scenarios ("This person is a software engineer. What pronoun do you use?") and analyze if the bot exhibits stereotypes (e.g., “he” for engineers, “she” for HR roles). Metrics like WEAT (Word Embedding Association Test), bias ladders, and disparity scores quantify model bias across occupations, pronouns, and sentiment.

    Remediation involves both pre- and post-processing techniques. In training, implement counterfactual data augmentation—introduce examples where women are engineers and men are in HR—so biases are disassociated from gender. Use fairness-aware loss functions or adversarial training to penalize the model for biased associations. After deployment, apply output filtering—post-process responses and flag or rewrite those that contain gendered stereotypes. Ongoing audits with human-in-the-loop review catch subtler biases and unintended edge cases.

    Additionally, system-level provisions like bias monitoring dashboards, frequent retraining with fresh and more balanced data, and clear reporting mechanisms for users can address emerging or context-dependent biases. Transparent communication of mitigation strategies to end-users and stakeholders builds trust and compliance with ethical guidelines and legal requirements.
    </p>
  </details>

  <details>
    <summary>What are LangChain, LangGrpah, Llama index, etc.?</summary>
    <p>
    LangChain is an open-source framework for creating powerful LLM-based applications by building composable chains of operations—prompting, tool use, memory, and agent orchestration. It simplifies tasks like chaining multiple LLM calls, working with APIs, and integrating tools such as search engines or databases. LangChain supports modular construction, making it easy to test and swap components or expand workflows for advanced use cases.

    LangGraph extends this paradigm by providing graph-based (node/edge) workflows for multi-agent scenarios. It lets developers design complex, conditional execution paths and manage persistent state, which is essential for agentic AI that needs planning, tool switching, and multi-turn conversations.

    LlamaIndex (formerly GPT Index) bridges LLMs with external data sources—documents, PDFs, APIs, SQL databases—by ingesting, indexing, and enabling semantic retrieval over heterogeneous corpora. Its key features include document chunking, embedding, indexing strategies, and retriever models that supply context to LLMs, making them expert-aware and less prone to hallucination.

    Collectively, these frameworks empower developers to create end-to-end “AI pipelines” for tasks such as document Q&A, chatbots, contextual agents, and retrieval-augmented applications using standardized but flexible building blocks.
    </p>
  </details>

  <details>
    <summary>Classical NLP and related topics</summary>
    <p>
    Classical NLP comprises pre-deep learning approaches for handling human language, primarily using symbolic, rule-based, and statistical models. Key topics include tokenization (breaking text into words/subwords), stemming/lemmatization (reducing words to base forms), part-of-speech tagging, named entity recognition, syntactic parsing, and dependency analysis. Vector space models like TF-IDF allow for basic document retrieval and topic extraction, while approaches such as n-gram language models, Hidden Markov Models (HMM), and Conditional Random Fields (CRF) power sequence modeling and information extraction.

    Sentiment analysis, topic modeling (using LDA, NMF), and text classification (Naive Bayes, SVMs) were common before neural approaches. Classical NLP excels in interpretability, transparency, and operates efficiently on small datasets—a significant advantage for resource-constrained environments. Important concepts also include semantic similarity (using cosine similarity), information retrieval (using BM25 or Lucene), and finite state automata for basic parsing.

    These techniques underpin many preprocessing steps, data normalization routines, and even feature extraction pipelines used in modern deep learning-based NLP. Understanding them is crucial for debugging, auditing, and integrating domain knowledge into larger generative or hybrid systems.
    </p>
  </details>

  <details>
    <summary>How to handle system failures?</summary>
    <p>
    Managing system failures in GenAI solutions involves architectural resilience, rigorous monitoring, and robust recovery protocols. Start by designing for fault tolerance: use health checks, rate limiting, and circuit breakers to isolate failures so they don't cascade. For multi-component systems (retriever, generator, vector DB), deploy service meshes or orchestrators (like Kubernetes) for automated restarts, scaling, and failover.

    Graceful degradation ensures partial functionality—fallback to cached responses, simpler models, or even deterministic templates if the main LLM is unavailable. Implement persistent storage for key artifacts and context checkpoints, enabling state recovery after outages. Distributed tracing, structured logging, and real-time alerting (using systems like Prometheus and Grafana) facilitate rapid root-cause analysis and response.

    For data integrity, enforce idempotency in API calls to prevent repeated actions post-recovery. Establish comprehensive recovery playbooks/runbooks, and regularly test incident scenarios—like DR drills—for team preparedness. Conduct blameless post-mortems to continually improve system robustness.

    In production, it’s critical to separate concerns: don’t let LLM outages affect data pipelines, and vice versa. Proactively communicate with users and automatically escalate severe issues to engineering or incident management teams for rapid containment and resolution.
    </p>
  </details>

  <details>
    <summary>Difference between fine-tuning, prompt-engineering and RAG</summary>
    <p>
    Fine-tuning, prompt engineering, and RAG are key methods for adapting LLMs to specific needs, each with unique strengths and limitations. Fine-tuning retrains an LLM on domain or task-specific data, updating its weights so it “learns” new patterns. This achieves deep specialization and higher accuracy on narrow tasks, but requires significant data and compute, and risks overfitting or catastrophic forgetting.

    Prompt engineering doesn’t alter the model’s parameters; instead, it crafts the input prompt’s structure and wording to steer the model’s outputs. This is lightweight, cost-effective, and ideal for rapid experimentation or scenarios where weight modification isn’t possible, but relies on the LLM’s pre-existing knowledge and may lack reliability for complex tasks.

    Retrieval-Augmented Generation (RAG) combines LLMs with external retrieval systems, injecting the most relevant contextual information directly into the input for each generation. This enables dynamic adaptation to new or proprietary information without retraining or prompt adjustment, extending an LLM’s effective knowledge base and improving factuality.

    Each approach can be combined—for instance, fine-tuning a model, then incorporating prompt engineering or RAG on top for maximum flexibility and accuracy, tailored to organizational requirements and deployment constraints.
    </p>
  </details>

  <details>
    <summary>Context window management</summary>
    <p>
    Managing an LLM’s context window, which sets the maximum number of tokens (words/subwords) for input and output combined, is crucial for maintaining answer quality and session coherence in real-world applications. As conversations or documents grow, older or less relevant context may be omitted (“context overflow”), causing loss of essential information and decreased response fidelity.

    Various strategies exist to optimize within these constraints. Prompt truncation cuts context from the oldest turns, but can miss important references. Dynamic context selection prioritizes recent, relevant, or salient data using heuristics or retrieval models. Chunking breaks long documents into manageable, semantically meaningful segments (overlapping windows help preserve continuity), and can feed only the most pertinent chunks. Summarization condenses previous context to free up tokens while retaining functional meaning.

    Architectural solutions include external memory buffers, context-aware cache, or retrieval mechanisms (as with RAG). Frameworks like LangChain implement memory management primitives such as conversation buffers or retriever-augmented memories, automating context prioritization for seamless multi-turn exchanges.

    Careful management ensures LLMs can reason over long histories, maintain entity consistency, and reduce context-related hallucinations, directly impacting user experience and system robustness.
    </p>
  </details>

  <details>
    <summary>How would you evaluate the quality of responses of a LLM</summary>
    <p>
    Evaluating LLM-generated responses requires a holistic framework combining quantitative and qualitative methods. Quantitative metrics like BLEU, ROUGE, METEOR, and BERTScore gauge overlap or semantic similarity with reference answers, but these may not fully reflect response accuracy or context-appropriateness, especially for creative or open-ended outputs.

    Qualitative evaluation includes manual annotation by experts or lay users—grading responses on relevance, factual accuracy, completeness, coherence, style, and safety. In regulated or domain-specific uses (e.g., healthcare), domain experts benchmark against compliance, liability, and ethical standards. Dialogues are sometimes evaluated using dialogue-specific metrics like perplexity, conversational engagement, and dialog success rate.

    To scale, LLM-as-a-judge methods task a strong model with grading outputs, though this must be validated against human judgment to ensure reliability and avoid circular bias. Error-type analysis, such as cataloguing hallucinations, omissions, or harmful content, enables focused model improvement.

    In real-world applications, continuous evaluation is performed via monitoring user feedback, complaint rates, and long-term task success rates. Incorporating A/B tests and measuring user retention or task completion also provide actionable insights for iterative tuning.
    </p>
  </details>

  <details>
    <summary>Agentic AI and related topics</summary>
    <p>
    Agentic AI refers to systems or agents driven by LLMs that autonomously plan, make decisions, and interact with APIs or dynamic environments to accomplish complex tasks. Unlike stateless chatbots, agentic AI incorporates memory, state management, and contextual reasoning to pursue goals across multiple steps. Core building blocks include planning (sequencing sub-tasks), tool use (calling APIs, databases, or web services), event-driven workflows, and stateful memory to track progress or recall prior actions.

    Frameworks like LangChain, LangGraph, CrewAI, and Semantic Kernel provide primitives for managing multi-agent systems, orchestrating interactions, failure recovery, and ensuring parallel or conditional executions. Agents can “delegate” subtasks to other agents or tools, process asynchronous events, and learn from user corrections.

    Real-world applications are vast: personal AI assistants, workflow automation, multi-modal agents (text, image, audio), and integration with business logic or external controls. Crucial challenges involve ensuring agents stay aligned with user goals and safety policies, don’t invoke tools in unsafe contexts, and provide explainable decision paths.

    Robust agentic AI systems feature permission policies, guardrails to restrict harmful tool use, and interpretability features for audit and debugging. As agentic systems evolve, they enable AI to take on real work—fetching and analyzing information, guiding users, or automating operational workflows with increasing autonomy.
    </p>
  </details>

  <details>
    <summary>How would you secure sensitive data like PII without sharing it with LLMs?</summary>
    <p>
    Securing sensitive data such as Personally Identifiable Information (PII) before LLM interaction involves a rigorous application of privacy engineering practices throughout the data pipeline. Start by applying Named Entity Recognition (NER) tools—like spaCy, Stanford NLP, or commercial APIs—to detect PII in text inputs. Once identified, use masking or redaction strategies to replace names, addresses, phone numbers, and other PII with generic tokens or pseudonyms before transmitting data to the LLM. For even stronger privacy, formal anonymization or pseudonymization frameworks (such as Microsoft’s Presidio) can ensure systematic consistency and compliance.

    In scenarios requiring original data post-LLM processing, maintain robust mapping tables protected by encryption and access controls, allowing controlled reversible pseudonymization. For cloud-based LLMs or external APIs, route traffic through privacy proxies or data loss prevention engines to enforce policy-based filtering or redaction, automatically blocking outbound sensitive content.

    For highly constrained environments, deploy LLMs within on-premises or virtual private cloud setups, ensuring full control over infrastructure, audit logging, and access. Enforce the principle of least privilege and maintain compliance with organizational and regulatory requirements (GDPR, HIPAA). Continuous monitoring, periodic privacy audits, and incident response plans are crucial for sustaining strong data security practices.
    </p>
  </details>

  <details>
    <summary>Anonymizers (Presidio)</summary>
    <p>
    Microsoft Presidio is a robust, open-source framework for detecting and anonymizing sensitive information, including PII, within natural language texts. Presidio leverages a combination of rule-based, pattern-based, and machine learning-powered Named Entity Recognition (NER) techniques to detect names, locations, organization references, dates, contact details, and more. It integrates configurable recognizers (detecting specific entity types), logic for risk scoring, and customizable anonymization actions like masking or token replacement.

    Presidio is designed to be modular and extensible. Developers can add custom recognizers, tune detection models for language-specific or domain-specific patterns, and define transformation pipelines for various downstream tasks. Crucially, Presidio can operate at scale—batch processing large datasets for redaction before storage, transfer, or LLM processing.

    Presidio supports REST APIs, making it straightforward to integrate into data ingestion workflows, chatbots, or customer support applications. By automating consistent and repeatable de-identification of sensitive data, Presidio helps organizations comply with regulatory frameworks like GDPR, HIPAA, and CCPA, and protects against data leakage in AI-driven systems. Presidio’s community and documentation make it accessible yet powerful in real-world privacy engineering efforts.
    </p>
  </details>

  <details>
    <summary>Vector DBs</summary>
    <p>
    Vector databases are specialized data management systems for indexing, searching, and managing high-dimensional vector embeddings produced by AI models from unstructured input like text, images, or audio. Traditional databases excel with precise key-value or SQL queries, but struggle with semantic searches where the goal is to find “similar” rather than exact matches. Vector DBs store numerical arrays—output from models like BERT or CLIP—and allow queries via similarity measures (e.g., cosine, inner product, Euclidean distance).

    These systems adopt approximate nearest neighbor (ANN) algorithms (e.g., HNSW, FAISS, IVF) to provide extremely fast similarity searches even at large scale (millions or billions of vectors). Common platforms include Pinecone, Milvus, Weaviate, Qdrant, and Chroma, offering horizontal scaling, metadata filtering, hybrid search (combining vectors and metadata), and real-time updates.

    In GenAI workflows, Vector DBs underpin retrieval-augmented generation (RAG), semantic search engines, content recommendation, and deduplication of generated outputs. By efficiently mapping input queries or user utterances to semantically related indexed contents in milliseconds, vector databases enable context-aware, accurate, and scalable AI applications.
    </p>
  </details>

  <details>
    <summary>Vector embeddings, searching using vectors and different chunking strategies</summary>
    <p>
    Vector embeddings transform complex data—like sentences or images—into dense numerical arrays that capture semantic meaning, enabling models to represent similarity in a geometric space. For example, “Paris” and “France’s capital” would have similar vector representations. When searching, a query input is embedded and compared to stored vectors in a database using metrics like cosine or Euclidean distance to surface the most semantically similar results.

    Chunking strategies determine how documents are divided before embedding and indexing. Fixed-size chunking slices text into blocks by word or character count, but may split meaningful phrases. Sentence-level or paragraph chunking preserves semantic units but can create uneven chunks. Recursive or overlap-based chunking, such as a sliding window approach, retains context across chunk boundaries, improving retrieval’s ability to capture multi-sentence relations. The chosen method directly affects semantic retrieval granularity, context recall, and performance.

    Optimized chunking minimises both the risk of context loss and redundancy. For QA or RAG, effective chunking translates to better matches and fewer hallucinations by LLMs, as retrieval supplies them the most pertinent and self-contained content fragments. Advanced orchestrators can dynamically select chunk sizes based on use case or query complexity, further tuning retrieval performance.
    </p>
  </details>

<!-- #################################################### The FAQ list ends here #################################################### -->

</details>
