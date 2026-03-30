# Chapter 3: The AI Landscape for Language Learning

---

## 3.1 Introduction: From Language Labs to Language Models

The history of technology in language education is, in many respects, a history of premature promises. Each wave of innovation -- the language laboratory, the personal computer, the internet, the smartphone -- arrived accompanied by predictions of pedagogical transformation that the technology ultimately could not sustain. The language lab did not replace the teacher. CALL software did not individualize instruction. Computer-mediated communication did not produce a generation of global citizens fluent in multiple languages. In each case, the technology delivered genuine but modest benefits that fell well short of the revolutionary claims made on its behalf.

This history counsels skepticism toward any new technology, including artificial intelligence. The burden of proof must fall on the technology and its proponents, not on the skeptics who demand evidence. Accordingly, this chapter begins not with what AI *can* do -- the capabilities are real and, in many cases, remarkable -- but with the structural limitations, known failure modes, and unresolved questions that constrain AI's contribution to language learning. Only after establishing these constraints does the chapter survey the current technology landscape and identify the domains in which AI demonstrates genuine promise.

This ordering -- limitations before affordances -- is deliberate. The applied linguistics community has been subjected to three years of breathless AI advocacy from technology companies, popular media, and well-intentioned but theoretically uninformed practitioners. The corrective is not dismissal but discipline: a systematic, SLA-theory-informed analysis of what contemporary AI systems actually do, how they do it, and where the gap between capability and pedagogical effectiveness remains wide.

---

## 3.2 From CALL to ICALL to AI-Powered Language Learning

### 3.2.1 The CALL Foundation

Computer-Assisted Language Learning, as reviewed in Chapter 1, evolved through three phases (Warschauer, 1996): Structural (behaviorist drill-and-practice), Communicative (skill-focused software enabling communicative tasks), and Integrative (internet-connected, multimedia, task-based environments). Each phase reflected the dominant language teaching methodology of its era and was constrained by the computational capabilities available.

Levy (1997) defined CALL broadly as "the search for and study of applications of the computer in language teaching and learning" (p. 1). This definition, capacious as it is, reveals the conceptual framework's limitation: it assumes the computer is an *application* -- a tool applied to language teaching by human designers for human learners. The computer assists; it does not participate. It delivers materials; it does not generate them. It scores responses; it does not understand them.

### 3.2.2 Intelligent CALL (ICALL)

The emergence of Natural Language Processing in the 1990s and 2000s enabled a class of CALL systems that could analyze learner language with some degree of linguistic sophistication. Heift and Schulze (2007) coined the term Intelligent CALL (ICALL) to describe systems incorporating NLP components -- primarily parsers and error analyzers -- that could diagnose specific grammatical errors and provide targeted feedback.

ICALL represented a meaningful advance. Where traditional CALL could only compare learner responses to a finite set of anticipated correct answers (often requiring exact string matching), ICALL systems could parse learner sentences, identify structural errors, and generate explanations referencing the underlying grammatical rules. Systems such as E-Tutor for German (Heift, 2004), Robo-Sensei for Japanese (Nagata, 2002), and the TAGARELA system for Portuguese (Amaral & Meurers, 2011) demonstrated that parser-based feedback could promote grammatical development in specific, constrained domains.

However, ICALL systems were brittle. Their parsers typically covered a subset of the target grammar, and learner input that fell outside the parser's coverage produced unhelpful or misleading feedback. The systems could not handle open-ended production, conversational interaction, or pragmatic evaluation. They were, in essence, sophisticated grammar checkers embedded in pedagogical frameworks -- valuable for specific instructional purposes but far from the adaptive, responsive language tutors that the field envisioned.

### 3.2.3 The AI Discontinuity

The advent of large language models in 2022-2023 produced what I characterized in Chapter 1 as a qualitative discontinuity in the CALL tradition. The discontinuity is not merely a matter of degree (better NLP, more accurate error detection) but of kind: for the first time, the technology can generate language, sustain conversation, and adapt its communicative behavior in real time. The shift from ICALL to AI-powered language learning is analogous to the shift from a calculator to a conversation partner: both involve computation, but the nature of the interaction is fundamentally different.

This does not mean that CALL and ICALL are obsolete. Much of the principled instructional design that characterized the best CALL research remains relevant, and the evaluation frameworks developed by Chapelle (2001) and others provide useful starting points for assessing AI tools. But the analytical framework must be extended to accommodate technologies that were not envisioned when these frameworks were created.

---

## 3.3 Current AI Technologies Relevant to Language Learning

### 3.3.1 Natural Language Processing (NLP)

Natural Language Processing is the subfield of AI concerned with enabling computers to process, analyze, and generate human language. For language learning, the most relevant NLP capabilities include:

**Tokenization and morphological analysis**: Breaking text into meaningful units (words, subwords, morphemes) and analyzing their grammatical properties. Modern tokenizers (e.g., Byte-Pair Encoding; Sennrich et al., 2016) operate at the subword level, enabling LLMs to handle morphologically complex languages, rare words, and neologisms. For language learning, this capability underlies vocabulary analysis tools, frequency profilers, and readability analyzers.

**Part-of-speech tagging and syntactic parsing**: Assigning grammatical categories to words and analyzing sentence structure. These capabilities enable automated grammar checking, error analysis, and the generation of grammatical explanations. State-of-the-art parsers achieve accuracy above 95% on standard benchmarks for well-resourced languages (Kitaev et al., 2019), though performance degrades for learner language, which contains errors and non-standard constructions that violate the parser's training distribution.

**Named entity recognition and information extraction**: Identifying and classifying entities (people, places, organizations, dates) in text. For language learning, these capabilities support content-based instruction, reading comprehension activities, and the generation of context-specific vocabulary exercises.

**Sentiment analysis and pragmatic evaluation**: Assessing the emotional tone, register, and pragmatic appropriateness of text. These capabilities are relevant to sociolinguistic and pragmatic instruction, though current systems perform unevenly across languages and cultural contexts. Pragmatic evaluation -- assessing whether an utterance is appropriate for a given social situation -- remains one of the most challenging NLP tasks and one where AI systems regularly fail (Taguchi & Roever, 2017).

### 3.3.2 Automatic Speech Recognition (ASR)

Automatic Speech Recognition converts spoken language into text. The current state of the art is represented by systems such as OpenAI's Whisper (Radford et al., 2023), Google's Universal Speech Model (Zhang et al., 2023), and Meta's Massively Multilingual Speech (Pratap et al., 2024). These systems achieve word error rates below 5% on clean English speech and increasingly competitive performance across dozens of languages.

For language learning, ASR enables:

- **Speech-to-text for pronunciation assessment**: Comparing the learner's spoken output to a target transcription to identify segmental and suprasegmental errors
- **Voice-based chatbot interaction**: Enabling spoken conversation with AI tutors
- **Dictation and transcription exercises**: Converting learner speech for subsequent written analysis
- **Accessibility**: Supporting learners who prefer oral over written interaction

The limitations of ASR for language learning are significant and well-documented. ASR systems are trained predominantly on native speaker data and perform substantially worse on accented speech, particularly from speakers whose L1 is typologically distant from the target language (Feng et al., 2021). This bias has direct consequences for pronunciation assessment: a system that cannot accurately recognize a learner's speech will provide inaccurate feedback. Moreover, ASR operates at the level of word recognition rather than phonological analysis: it can determine that the learner said "ship" instead of "sheep" but cannot diagnose the specific articulatory or perceptual process that produced the error. Chapter 8 examines these limitations in depth.

### 3.3.3 Natural Language Generation (NLG)

Natural Language Generation -- the production of coherent, contextually appropriate text by AI systems -- is the capability that most directly transforms the language learning landscape. Prior to LLMs, NLG was limited to template-based systems that filled slots in pre-defined sentence structures (e.g., "The weather in [city] today is [condition] with temperatures of [number] degrees"). These systems could generate weather reports and sports summaries but could not sustain a conversation, write a paragraph of expository prose, or produce a graded reading passage on an arbitrary topic.

LLMs generate text through next-token prediction: given a sequence of tokens, the model predicts the probability distribution over the vocabulary for the next token, samples from this distribution, appends the selected token to the sequence, and repeats. This autoregressive process produces text that is, in most cases, grammatically well-formed, contextually coherent, and stylistically fluent. The text reflects the distributional patterns of the training data, which for large models encompasses a significant fraction of the publicly available internet in multiple languages.

For language learning, NLG enables capabilities that were simply impossible before 2022:

- **On-demand comprehensible input**: Generating reading passages at any proficiency level, on any topic, in any register
- **Conversational interaction**: Sustaining open-ended dialogue in the target language, with the ability to adapt to the learner's proficiency, interests, and communicative goals
- **Corrective feedback with explanations**: Identifying errors in learner production and generating metalinguistic explanations in the learner's L1 or the target language
- **Task and exercise generation**: Creating communicative activities, grammar exercises, vocabulary quizzes, and assessment items dynamically
- **Role-play and simulation**: Assuming personas (hotel receptionist, job interviewer, doctor, classmate) and maintaining them across extended conversations

### 3.3.4 Large Language Models (LLMs)

Large Language Models deserve a more detailed technical treatment because they underpin most of the AI language learning applications discussed in this volume. The reader need not become a machine learning engineer, but a conceptual understanding of how LLMs work is essential for evaluating their strengths and limitations as language learning tools.

**Architecture**: All major LLMs are built on the transformer architecture (Vaswani et al., 2017). The key innovation of the transformer is the *self-attention mechanism*, which allows the model to weigh the relevance of every token in the input sequence to every other token when computing representations. This enables the model to capture long-range dependencies -- relationships between words that are distant in the sentence -- without the sequential processing bottleneck of recurrent architectures.

**Training**: LLMs are trained in two phases. In *pre-training*, the model processes enormous text corpora (hundreds of billions to trillions of tokens) using a self-supervised objective: predict the next token (for autoregressive models like GPT) or predict masked tokens (for bidirectional models like BERT). Pre-training produces a model with broad linguistic competence across languages and domains but no specific instruction-following behavior. In *fine-tuning*, the pre-trained model is adapted for specific tasks through supervised learning on curated datasets and/or reinforcement learning from human feedback (RLHF; Ouyang et al., 2022). Fine-tuning transforms a text completion engine into a conversational assistant, a translation system, or a language tutor.

**Emergent capabilities**: A defining characteristic of LLMs is the emergence of capabilities that were not explicitly trained. GPT-3, trained only to predict the next token, demonstrated the ability to translate between languages, answer questions, perform arithmetic, and generate code -- none of which were explicit training objectives (Brown et al., 2020). These emergent capabilities suggest that the pre-training process extracts more structure from language data than the training objective alone would predict. For language learning, the most relevant emergent capabilities are pragmatic sensitivity (adapting register and formality to context), metalinguistic explanation (articulating grammatical rules when prompted), and pedagogical scaffolding (adjusting complexity based on interlocutor proficiency).

**What LLMs do not have**: It is equally important to specify what LLMs lack. They do not have beliefs, desires, intentions, or communicative goals. They do not have a model of the interlocutor's knowledge state, emotional condition, or learning needs, except insofar as they can infer these from the conversational context. They do not have embodied experience, social identity, or cultural membership. They do not have a persistent memory of past interactions (beyond the context window of a single session, unless augmented with external memory systems). They do not have a theory of language acquisition. Their output is generated through statistical pattern matching, not through rule application, communicative planning, or pedagogical reasoning. These absences do not preclude their utility for language learning, but they constrain it in ways that must be acknowledged.

### 3.3.5 Multimodal AI

The convergence of text, speech, image, and video processing within unified AI systems represents the most recent significant development. Multimodal models such as GPT-4o (OpenAI, 2024) and Gemini (Google DeepMind, 2024) can:

- Process a learner's spoken utterance, evaluate its pronunciation, and respond with synthesized speech -- all within a single model
- Analyze an image (a photograph, a scene, a document) and generate target-language descriptions, questions, or vocabulary exercises based on its content
- Process video input and generate comprehension questions, cultural commentary, or transcription exercises
- Integrate text and audio to provide synchronized reading-listening experiences with real-time glossing

For language learning, multimodality addresses a longstanding limitation of text-based AI systems: language learning is inherently multimodal, involving listening, speaking, reading, and writing in combination with visual, gestural, and contextual cues. A multimodal AI system can, in principle, provide an integrated learning experience that approaches the richness of immersive human interaction. In practice, the quality of multimodal integration varies considerably, and the field is in its early stages. The most mature multimodal applications are in speech-to-text and text-to-speech; image and video processing for language learning remain experimental.

---

## 3.4 Major Platforms and Tools

### 3.4.1 Comprehensive Language Learning Platforms

**Duolingo** (founded 2011; over 500 million registered users by 2024) is the world's most widely used language learning application. Its core pedagogical model is a gamified sequence of discrete-point exercises -- translation, fill-in-the-blank, multiple choice, listening, and speaking -- organized into a skill tree with adaptive sequencing. Duolingo's AI integration has evolved through several stages: early versions used rule-based exercise templates; current versions employ machine learning for exercise selection and spaced repetition optimization (Settles & Meeder, 2016); and the premium tier (Duolingo Max) integrates GPT-4 for two features: "Explain My Answer" (metalinguistic explanations of exercise results) and "Roleplay" (open-ended conversation practice).

From an SLA-theoretical perspective, Duolingo's strengths lie in its operationalization of Skill Acquisition Theory's emphasis on extensive practice and its exploitation of frequency effects consistent with usage-based approaches. Its limitations are equally clear: the exercise format constrains output to single sentences or short phrases (limiting the pushed output that Swain's hypothesis values), interaction is human-to-machine rather than negotiated (limiting the interactional modifications that Long's hypothesis identifies as facilitative), and the gamification structure may promote engagement without ensuring the depth of processing that Schmidt's Noticing Hypothesis requires.

**Babbel** (founded 2007; approximately 10 million subscribers) takes a more explicitly pedagogical approach, with lessons designed by linguists and organized around communicative topics. Babbel's AI integration includes speech recognition for pronunciation practice and adaptive review systems. Its SLA orientation is more communicative than Duolingo's: lessons emphasize functional language use in real-world scenarios, and the curriculum is structured around discourse functions (ordering food, asking directions, making appointments) rather than grammatical sequences.

**Busuu** (founded 2008; over 120 million users) integrates AI features with a social learning component: learners can submit writing and speaking exercises for correction by native speakers in the Busuu community. This hybrid model -- AI for adaptive practice, humans for authentic interaction and feedback -- is theoretically promising because it addresses the limitations of AI-only interaction (absence of genuine communication) while leveraging AI's advantages (availability, adaptivity, patience).

### 3.4.2 AI-Native Language Learning Platforms

A new generation of platforms, launched since 2022, treats AI not as an enhancement to a traditional curriculum but as the core pedagogical engine.

**Speak** (founded 2016; launched AI-powered features 2022) focuses on spoken language production, using ASR and LLMs to provide real-time conversational practice with corrective feedback. Speak's pedagogical model emphasizes output practice -- the learner speaks more than they listen -- which aligns with Swain's Output Hypothesis and DeKeyser's emphasis on productive practice. The system provides immediate feedback on pronunciation and grammar, adjusts conversation difficulty based on learner performance, and offers structured lessons that progress from guided practice to free conversation.

**TalkPal** (launched 2023) provides AI-powered conversation practice across multiple languages, with features including role-play scenarios, debate practice, and topic-based conversations. TalkPal's strength lies in the variety of its conversational contexts, which provide the kind of contextualized, communicatively meaningful practice that Skill Acquisition Theory prescribes.

**Languagefly**, **Lingvist**, and similar platforms employ adaptive algorithms to optimize vocabulary acquisition and grammar practice, drawing on spaced-repetition research and AI-powered content generation.

### 3.4.3 General-Purpose AI as Language Learning Tool

Perhaps the most significant development in AI-mediated language learning is the widespread adoption of general-purpose AI systems -- ChatGPT, Claude, Gemini, and their competitors -- as language learning tools. These systems were not designed for language instruction, but their conversational capabilities, multilingual proficiency, and ability to follow complex instructions make them remarkably versatile language tutors when prompted appropriately.

A learner who instructs ChatGPT to "Act as my Spanish tutor. Speak to me only in Spanish at a B1 level. Correct my errors by providing the correct form and a brief explanation in English. If I make the same error three times, give a more detailed grammatical explanation" has, in effect, configured a personalized language tutoring system with a specific pedagogical approach (corrective feedback with escalating explicitness) and a proficiency-adaptive interaction model. This is *prompt engineering as instructional design*, and it represents a fundamental shift in the locus of pedagogical control: from the platform designer to the learner (or teacher) who crafts the prompt.

The implications are profound. For the first time, a learner with no training in instructional design, SLA theory, or AI engineering can configure a language learning environment that approximates many of the features that decades of CALL research identified as desirable: comprehensible input, interactional feedback, pushed output, metalinguistic explanation, and adaptive difficulty. The question is whether this learner-configured environment is *good enough* -- whether the pedagogical intuitions of untrained users produce interactions that SLA theory would endorse.

The evidence is mixed. Learners who prompt AI systems for conversation practice report high satisfaction and engagement (Yan, 2023). However, without SLA-informed prompting, AI conversations tend to be accommodating rather than challenging: the AI agrees, elaborates, and moves on rather than pushing the learner to self-correct, providing sustained corrective feedback, or creating the kind of communicative pressure that Long's Interaction Hypothesis identifies as facilitative. The AI's default behavior is to be helpful, which in conversational terms means reducing friction -- precisely the opposite of what the Output Hypothesis and the Interaction Hypothesis suggest is needed for acquisition.

### 3.4.4 Machine Translation as Language Learning Tool

Google Translate, DeepL, and other neural machine translation (NMT) systems have achieved a level of quality that fundamentally changes their pedagogical status. Rule-based and statistical MT systems produced output that was obviously machine-generated -- stilted, frequently incorrect, and pragmatically inappropriate. Learners who used these systems were, in effect, practicing bad habits. Neural MT systems, by contrast, produce output that is often fluent, idiomatic, and pragmatically appropriate -- particularly for well-resourced language pairs (English-Spanish, English-French, English-German, English-Chinese).

This quality improvement creates a pedagogical dilemma. If MT output is good enough to be indistinguishable from competent human translation, then learners can use it as a *crutch* -- producing target-language text without the cognitive effort that acquisition requires (Swain, 1995). Teachers have long warned against this, and many classroom policies prohibit MT use. However, if MT output is good enough to serve as comprehensible input, then learners can also use it as a *scaffold* -- comparing their own attempted translations against MT output to notice gaps, test hypotheses, and develop metalinguistic awareness (Lee, 2020).

The distinction between crutch and scaffold depends not on the technology but on the task design and the learner's orientation. A learner who copies MT output into an assignment is using it as a crutch. A learner who writes a draft, compares it to MT output, identifies discrepancies, and revises based on the comparison is using it as a scaffold. Pedagogically informed task design can guide learners toward the latter use, and AI tools can be configured to support scaffolded MT use (e.g., by providing MT output only after the learner has attempted their own translation).

---

## 3.5 Critical Analysis: What AI Does Well

Having established the technology landscape, we can now assess AI's genuine strengths for language learning -- capabilities that are empirically supported and theoretically grounded.

### 3.5.1 Availability and Patience

The most mundane advantage of AI language tools is also, for many learners, the most consequential: AI is always available and never impatient. For learners who lack access to human interlocutors in the target language -- a common situation for foreign language learners in monolingual communities -- AI provides the only viable source of conversational practice outside the classroom. For learners who are anxious about speaking with humans, AI provides a low-stakes environment for initial practice.

This advantage should not be underestimated. The practice deficit identified by Skill Acquisition Theory (DeKeyser, 2007) is the single most significant constraint on instructed SLA: learners simply do not produce enough target language, in enough contexts, with enough feedback, to develop procedural knowledge. If AI partially addresses this deficit by providing unlimited, patient, corrective practice, the impact on acquisition could be substantial -- even if the quality of AI interaction is inferior to human interaction on every other dimension.

### 3.5.2 Adaptive Input Generation

AI systems can generate comprehensible input calibrated to the learner's proficiency level with a precision that no human teacher can match across an entire class. An AI system that has assessed the learner's vocabulary size, grammatical competence, and reading level can produce texts that target the optimal i+1 zone for that specific learner. This capability addresses one of the fundamental challenges of classroom instruction: the heterogeneity of learner proficiency levels, which means that any given text or lecture is too easy for some students and too hard for others.

The quality of AI-generated input has improved dramatically since 2023. Current LLMs produce text that is grammatically well-formed, lexically appropriate, and stylistically varied. They can generate input in specific registers (formal, informal, academic, conversational), on specific topics (news, science, culture, daily life), and in specific genres (narrative, expository, dialogue, email). They can embed target vocabulary and grammatical structures at controlled frequencies, creating the kind of input flood and input enhancement that SLA research has identified as facilitative of acquisition (Trahey & White, 1993; Sharwood Smith, 1993).

### 3.5.3 Immediate, Detailed Corrective Feedback

AI systems can provide corrective feedback that is immediate, specific, and metalinguistically detailed. When a learner produces an error, an AI tutor can identify the error type (morphological, syntactic, lexical, pragmatic), provide the correct form, explain the relevant rule, offer additional examples, and generate practice activities targeting the same structure -- all within seconds.

The SLA literature on corrective feedback consistently finds that explicit feedback with metalinguistic explanation is more effective than implicit feedback for certain learner populations and certain target structures (Li, 2010; Lyster & Saito, 2010). AI systems excel at explicit, metalinguistic feedback. They can also produce recasts (implicit reformulations) that, while lacking the social and communicative context of human recasts, provide the form-form juxtaposition that Schmidt's Noticing Hypothesis identifies as the mechanism through which recasts facilitate acquisition.

### 3.5.4 Scalability and Equity

AI democratizes access to language learning resources that have historically been available only to privileged learners. A high-quality human language tutor costs $30-100 per hour; an AI language tutor costs a monthly subscription of $10-30 or is available for free. An immersive language learning program (study abroad, intensive language institute) costs thousands of dollars and requires weeks or months of dedicated time; AI-mediated immersion simulation is available on a smartphone. A native speaker conversation partner requires geographic proximity or scheduled online meetings; an AI conversation partner is available anywhere, anytime.

These cost and access advantages are not peripheral. For learners in low-resource educational settings -- rural communities, under-resourced schools, developing countries with limited foreign language teaching infrastructure -- AI may provide access to language learning opportunities that would otherwise not exist. The equity implications are significant and deserve more attention than they have received in the SLA literature, which has historically focused on learners in well-resourced university and school contexts.

---

## 3.6 Critical Analysis: What AI Cannot Do

### 3.6.1 Genuine Communication

AI systems do not communicate. They generate text that *resembles* communication -- that has the surface features of conversational exchange, including turn-taking, topic management, and apparent responsiveness to the interlocutor -- but they do not have communicative intentions, information needs, or messages to convey. When an AI chatbot asks the learner "What did you do this weekend?", it does not want to know. When it responds to the learner's answer with "That sounds wonderful!", it does not find it wonderful. When it asks a follow-up question, it is generating a statistically likely continuation, not pursuing genuine curiosity.

This matters for SLA because many theoretical constructs assume that language learning occurs in the context of genuine communication. Long's (1996) Interaction Hypothesis specifies that negotiation of meaning facilitates acquisition; negotiation of meaning presupposes that both participants have meaning to negotiate. Norton's (2013) investment theory argues that learners invest in language learning because they seek access to material and symbolic resources; AI interaction offers no such resources. Kramsch's (2009) concept of the "multilingual subject" situates language learning within the learner's identity project; AI interaction, stripped of social risk and social reward, may not engage the identity dimensions of language learning.

The counterargument -- that the *appearance* of communication may trigger the same cognitive processes as genuine communication -- is plausible but unproven. If acquisition depends on cognitive mechanisms (noticing, hypothesis testing, form-meaning mapping) that can be triggered by simulated communication, then AI may be effective. If acquisition depends on social mechanisms (investment, identity negotiation, legitimate peripheral participation) that require authentic human relationships, then AI's contribution is inherently limited. The most likely reality is that both cognitive and social mechanisms contribute, and AI serves the former better than the latter.

### 3.6.2 Pragmatic Competence

Pragmatic competence -- the ability to use language appropriately in social context -- is one of the most difficult aspects of L2 development and one where AI systems are weakest. Pragmatics encompasses speech acts (requesting, apologizing, complimenting), politeness strategies (directness, indirectness, deference, solidarity), register variation (formal vs. informal), and sociopragmatic knowledge (understanding the social norms and power dynamics that govern language use in a particular community).

AI systems can produce pragmatically appropriate language in many contexts, drawing on patterns in their training data. But they cannot teach pragmatic competence in the fullest sense because they cannot model the social consequences of pragmatic failure. When a learner uses an inappropriately direct request with a human interlocutor, the interlocutor's reaction -- a raised eyebrow, a stiffened posture, an awkward pause -- provides immediate, embodied feedback on the pragmatic violation. An AI system can be programmed to flag pragmatic inappropriateness, but this flagging is metalinguistic rather than social: it tells the learner that their utterance was inappropriate, but it does not create the social experience of inappropriateness that motivates pragmatic development.

Moreover, pragmatic norms are culturally specific, community-specific, and context-dependent in ways that training data cannot fully capture. An AI system trained on internet text reflects the pragmatic norms of internet communication, which are not the pragmatic norms of face-to-face interaction, professional communication, or academic discourse. Taguchi and Roever (2017) demonstrated that pragmatic competence develops through participation in communities of practice -- sustained engagement with the social norms and communicative routines of a target community. AI cannot provide this participation.

### 3.6.3 Cultural Knowledge and Intercultural Competence

Language learning is inseparable from cultural learning. Kramsch (1993) argued that language teaching should develop "intercultural competence" -- the ability to mediate between one's own culture and the target culture, to recognize cultural differences, and to navigate cross-cultural communication effectively. AI systems possess encyclopedic knowledge about cultures but lack the experiential, embodied, and relational understanding that characterizes genuine intercultural competence.

An AI system can provide accurate information about Japanese honorifics, explain the cultural significance of *tatemae* and *honne*, and generate contextually appropriate examples of formal Japanese speech. What it cannot do is help the learner *experience* the social discomfort of violating honorific norms, or navigate the ambiguity of a conversation in which the interlocutor's words and intentions diverge, or develop the empathetic perspective-taking that intercultural competence requires. Cultural learning, like pragmatic learning, is fundamentally social: it occurs through participation in cultural practices, not through information about them.

### 3.6.4 Handling Learner Interlanguage

A pervasive and underappreciated limitation of current AI systems is their difficulty in processing *learner interlanguage* -- the systematic but non-target-like language that L2 learners produce at various developmental stages. LLMs are trained predominantly on text produced by proficient (usually native) speakers. Learner language -- with its grammatical errors, L1 transfer effects, developmental patterns, and creative constructions -- falls outside the training distribution.

This has several consequences. First, ASR systems struggle to recognize heavily accented speech, producing transcription errors that cascade into incorrect feedback. Second, LLMs sometimes fail to identify errors in learner writing because they interpret the learner's intended meaning rather than evaluating the form -- a pragmatically generous behavior that is unhelpful when the purpose of the interaction is error correction. Third, AI systems may provide feedback that is technically correct but developmentally inappropriate -- correcting an error that the learner is not yet developmentally ready to acquire (Pienemann, 1998).

### 3.6.5 Hallucination and Factual Unreliability

LLMs "hallucinate" -- they generate text that is fluent and confident but factually incorrect. In general-purpose applications, this is a reliability concern. In language learning, it is a pedagogical hazard. An LLM providing a grammatical explanation may state a rule that does not exist, cite an exception that is not real, or describe a usage pattern that is nonstandard. A learner who trusts the AI's explanation may internalize incorrect linguistic knowledge.

The hallucination problem is particularly acute for languages with complex morphological systems (Arabic, Turkish, Finnish), less-resourced languages (where the training data is sparse), and pragmatic/cultural knowledge (where the "correct" answer depends on context). Designing AI language learning systems that are reliably accurate -- or that clearly signal uncertainty when they are not -- remains an unsolved engineering challenge.

### 3.6.6 The Low-Resource Language Problem

AI systems perform best on well-resourced languages -- primarily English, but also Chinese, Spanish, French, German, Japanese, Korean, and a few dozen others for which large training corpora exist. For the vast majority of the world's approximately 7,000 languages, AI capabilities range from limited to nonexistent.

Joshi et al. (2020) categorized the world's languages into five groups based on the availability of digital language resources: from "winners" (English, with billions of tokens of training data) to "left-behinds" (thousands of languages with essentially no digital presence). For languages in the lower categories, LLMs produce unreliable output, ASR systems fail to recognize speech, and MT systems produce translations that are more misleading than helpful.

This has equity implications that the AI-SLA community must confront. If AI-powered language learning is available only for well-resourced languages, it will reinforce the existing linguistic hierarchy rather than challenging it. Learners of English, Spanish, or Mandarin will benefit from AI tools; learners of Quechua, Yoruba, or Hmong will not. Indigenous and minority language communities, which face the greatest challenges in language maintenance and revitalization, are precisely the communities for which AI tools are least available.

---

## 3.7 Ethical Considerations

### 3.7.1 Data Privacy and Learner Surveillance

AI language learning systems collect detailed data about learner behavior: every keystroke, every spoken utterance, every error, every pause, every repeated item. This data is pedagogically valuable -- it enables adaptive algorithms to personalize the learning experience -- but it also creates surveillance risks. Learner data may be used for purposes beyond instruction (targeted advertising, profiling, sale to third parties), may be stored insecurely, and may be subject to data breaches.

The ethical framework for learner data in AI-mediated language learning is underdeveloped. FERPA (in the United States) and GDPR (in the European Union) provide baseline protections, but these regulations were not designed for the continuous, granular data collection that AI systems perform. Language learning data is particularly sensitive because it reveals the learner's L1 (and therefore, often, their national origin or ethnicity), their proficiency level (which may affect employment or immigration decisions), and their communicative behavior (which may reveal personal information disclosed during conversation practice).

### 3.7.2 Bias and Representation

AI systems reflect the biases present in their training data. For language learning, relevant biases include:

**Linguistic bias**: LLMs perform better on standardized, prestige varieties of languages (Standard American English, Castilian Spanish, Mandarin Chinese) than on non-standard varieties, dialects, and sociolects. Learners who aspire to non-standard varieties -- African American Vernacular English, Andalusian Spanish, Cantonese -- receive less accurate AI support.

**Cultural bias**: AI-generated content reflects the cultural perspectives dominant in the training data, which is disproportionately Western, English-language, and middle-class. Cultural representations of target-language communities may be stereotypical, superficial, or inaccurate.

**Accent bias in ASR**: As noted above, ASR systems perform worse on accented speech, which means that learners who most need pronunciation feedback -- those whose pronunciation diverges significantly from the training norm -- receive the least accurate feedback.

**Gender and identity bias**: AI-generated language examples, conversation scenarios, and cultural descriptions may reflect gender stereotypes, heteronormative assumptions, and other biases that are problematic in educational contexts.

### 3.7.3 Academic Integrity

The ability of AI systems to produce fluent target-language text raises fundamental questions about academic integrity in language courses. If a student uses ChatGPT to write an essay in Spanish, has the student demonstrated Spanish writing competence? If a student uses an AI speaking coach to prepare for an oral exam, is the exam measuring the student's competence or the AI's coaching effectiveness?

These questions do not have simple answers. The boundary between legitimate tool use (using a dictionary, using a grammar reference) and illegitimate tool use (having someone else write your essay) has always been negotiated socially and institutionally. AI blurs this boundary further because it can provide assistance at every point on the continuum, from looking up a single word to generating entire texts.

The pedagogical response to AI-assisted language production should be informed by SLA theory, not by knee-jerk prohibition. If the goal of a writing assignment is to promote the noticing, hypothesis-testing, and metalinguistic reflection that Swain (1995) identified as functions of output, then the assignment should be designed so that AI assistance does not short-circuit these processes. This may mean redesigning assessments to emphasize process over product -- evaluating drafts, self-corrections, and reflective journals rather than final texts.

### 3.7.4 The Deskilling of Language Teachers

A concern frequently voiced by language educators is that AI will render human teachers obsolete. This concern is, in my assessment, misplaced but not entirely without foundation. AI cannot replace the social, cultural, and relational dimensions of language teaching that the theories reviewed in Chapter 2 identify as critical to acquisition. But AI *can* replace certain functions that currently consume a large portion of teachers' time: generating exercises, grading discrete-point assessments, providing basic corrective feedback on written work, and leading pronunciation drills.

The risk is not that AI will replace teachers but that it will *deskill* them -- that administrators, attracted by cost savings, will reduce teacher training, class time, and professional development budgets on the assumption that AI can compensate. If this occurs, the human dimensions of language teaching that AI cannot replace will be attenuated without being eliminated, producing a learning environment that is technologically rich but pedagogically impoverished.

The appropriate response is not to resist AI integration but to redefine the teacher's role in AI-augmented language instruction. The teacher's unique contributions -- providing authentic communication, modeling intercultural competence, addressing the affective and identity dimensions of language learning, designing tasks that leverage AI's strengths while compensating for its weaknesses -- become more important, not less, in an AI-rich environment. Teacher education programs must prepare language teachers to be informed consumers and critical evaluators of AI tools, not passive implementers of technology mandates.

### 3.7.5 Dependency and the Atrophy of Learning Strategies

A final ethical concern that SLA theory illuminates: AI may create a dependency that undermines the development of autonomous learning strategies. Effective language learners develop metacognitive strategies for managing their own learning: they identify their weaknesses, seek out appropriate input, monitor their comprehension, and self-correct their production (Oxford, 1990; Cohen, 2011). These strategies are not merely instrumental; they are acquisitionally productive because they require the learner to engage actively with the learning process.

AI tools that provide seamless, frictionless support may obviate the need for these strategies. If the AI identifies weaknesses, selects input, monitors comprehension, and corrects production, the learner is relieved of the metacognitive work that strategy development requires. The short-term effect is a smoother learning experience; the long-term effect may be a learner who is unable to function without AI support -- who has acquired language competence but not language learning competence.

This concern aligns with Benson's (2011) concept of *learner autonomy* -- the capacity to take charge of one's own learning -- which many applied linguists consider a goal of language education in its own right, not merely a means to linguistic competence. Designing AI tools that promote autonomy rather than dependency requires deliberate pedagogical choices: gradually reducing support, prompting self-assessment, and creating tasks that require the learner to make independent decisions about their learning.

---

## 3.8 A Framework for Evaluating AI Language Learning Tools

Drawing on the theoretical foundations of Chapter 2 and the critical analysis of this chapter, I propose a preliminary evaluation framework for AI language learning tools. This framework extends Chapelle's (2001) CALL evaluation criteria for the AI era:

1. **SLA-Theoretical Grounding**: Does the tool engage with established SLA constructs (comprehensible input, interaction, output, feedback, noticing)? Can its pedagogical approach be articulated in theoretical terms?

2. **Adaptive Calibration**: Does the tool adapt to the individual learner's proficiency level, L1 background, learning goals, and developmental readiness? How accurate is this adaptation?

3. **Output Elicitation**: Does the tool push learners to produce language, or does it primarily provide input and receptive activities? Does it scaffold output without eliminating productive struggle?

4. **Feedback Quality**: Does the tool provide corrective feedback? What types (recasts, explicit correction, metalinguistic explanation)? Is the feedback accurate, timely, and appropriate to the learner's developmental level?

5. **Communicative Authenticity**: Does the tool create conditions for meaningful communication, or does it recapitulate drill-and-practice in a conversational wrapper? Does it provide tasks with genuine information gaps?

6. **Linguistic Accuracy**: Is the language generated by the tool grammatically, lexically, and pragmatically accurate in the target language? How does it handle low-frequency structures, dialectal variation, and pragmatic nuance?

7. **Autonomy Promotion**: Does the tool develop learner autonomy, or does it create dependency? Does it gradually withdraw support and promote self-directed learning?

8. **Equity and Access**: Is the tool available and effective for diverse learner populations? Does it support languages beyond English? Is it affordable and accessible in low-resource settings?

9. **Ethical Data Practices**: Does the tool collect learner data responsibly? Is data use transparent? Are privacy protections adequate?

10. **Empirical Evidence**: Has the tool been evaluated through rigorous, SLA-theory-informed research? Are learning outcomes measured through validated proficiency assessments, not merely engagement metrics?

This framework is not exhaustive, and subsequent chapters will elaborate specific criteria for specific domains (pronunciation assessment in Chapter 8, writing feedback in Chapter 7, assessment in Chapter 11). But it provides a starting point for the kind of principled, theory-driven evaluation that the field urgently needs.

---

## 3.9 Conclusion: Technology in Service of Theory

The AI landscape for language learning is vast, rapidly evolving, and deeply uneven. Some capabilities -- adaptive input generation, immediate corrective feedback, unlimited practice availability -- represent genuine advances that SLA theory can endorse and that empirical research should investigate. Other capabilities -- conversational simulation, pragmatic evaluation, cultural instruction -- remain limited in ways that current technology cannot overcome and that theoretical analysis illuminates.

The critical error, committed repeatedly in the history of CALL and now being repeated in the era of AI, is to evaluate technology on its own terms -- to ask what it can do rather than what learners need. SLA theory specifies what learners need: comprehensible input at the right level of challenge, interactional modifications that draw attention to form-meaning connections, opportunities for pushed output that force syntactic processing, corrective feedback that promotes noticing and hypothesis testing, scaffolded interaction within the ZPD that moves toward self-regulation, and authentic social contexts that engage the identity and investment dimensions of language learning.

AI can deliver some of these things effectively. It cannot deliver all of them. The chapters that follow examine, domain by domain, which theoretical needs AI can satisfy, which it can approximate, and which it cannot address at all. The measure of AI's value for language learning is not what the technology *does* but what the learner *acquires*.

---

## Discussion Questions

1. The chapter argues that the history of educational technology counsels skepticism toward AI claims. Identify one specific claim about AI language learning from a technology company or popular media source and evaluate it against the SLA theories reviewed in Chapter 2.

2. The chapter identifies general-purpose AI systems (ChatGPT, Claude, Gemini) as potentially more transformative for language learning than purpose-built language learning apps. What are the advantages and disadvantages of general-purpose AI versus purpose-built platforms for language instruction?

3. The evaluation framework in Section 3.8 proposes ten criteria for assessing AI language learning tools. Select a tool you have used (or are familiar with) and evaluate it against these criteria. Which criteria does it satisfy? Which does it fail?

4. The chapter discusses machine translation as both a "crutch" and a "scaffold." Design a classroom activity that uses machine translation as a scaffold for L2 writing development, specifying the task design features that prevent crutch use.

5. The low-resource language problem (Section 3.6.6) means that AI language learning tools are least available for the languages that most need support (endangered and minority languages). What technical and policy interventions could address this inequity?

6. Section 3.7.4 argues that AI risks "deskilling" language teachers. If you were designing a teacher education program for the AI era, what competencies would you prioritize? How would the teacher's role differ from the pre-AI era?

---

## References

Amaral, L. A., & Meurers, D. (2011). On using intelligent computer-assisted language learning in real-life foreign language teaching and learning. *ReCALL, 23*(1), 4-24.

Benson, P. (2011). *Teaching and researching autonomy* (2nd ed.). Pearson.

Brown, T. B., Mann, B., Ryder, N., Subbiah, M., Kaplan, J., Dhariwal, P., ... & Amodei, D. (2020). Language models are few-shot learners. *Advances in Neural Information Processing Systems, 33*, 1877-1901.

Chapelle, C. A. (2001). *Computer applications in second language acquisition: Foundations for teaching, testing, and research*. Cambridge University Press.

Cohen, A. D. (2011). *Strategies in learning and using a second language* (2nd ed.). Longman.

DeKeyser, R. M. (2007). *Practice in a second language: Perspectives from applied linguistics and cognitive psychology*. Cambridge University Press.

Feng, S., Kudina, O., Halpern, B. M., & Scharenborg, O. (2021). Quantifying bias in automatic speech recognition. *arXiv preprint arXiv:2103.15122*.

Heift, T. (2004). Corrective feedback and learner uptake in CALL. *ReCALL, 16*(2), 416-431.

Heift, T., & Schulze, M. (2007). *Errors and intelligence in computer-assisted language learning: Parsers and pedagogues*. Routledge.

Joshi, P., Santy, S., Buber, A., Bali, K., & Choudhury, M. (2020). The state and fate of linguistic diversity and inclusion in the NLP world. *Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics*, 6282-6293.

Kitaev, N., Cao, S., & Klein, D. (2019). Multilingual constituency parsing with self-attention and pre-training. *Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics*, 3499-3505.

Kramsch, C. (1993). *Context and culture in language teaching*. Oxford University Press.

Kramsch, C. (2009). *The multilingual subject*. Oxford University Press.

Lee, S. M. (2020). The impact of using machine translation on EFL students' writing. *Computer Assisted Language Learning, 33*(3), 157-175.

Levy, M. (1997). *Computer-assisted language learning: Context and conceptualization*. Oxford University Press.

Li, S. (2010). The effectiveness of corrective feedback in SLA: A meta-analysis. *Language Learning, 60*(2), 309-365.

Long, M. H. (1996). The role of the linguistic environment in second language acquisition. In W. C. Ritchie & T. K. Bhatia (Eds.), *Handbook of second language acquisition* (pp. 413-468). Academic Press.

Lyster, R., & Saito, K. (2010). Oral feedback in classroom SLA: A meta-analysis. *Studies in Second Language Acquisition, 32*(2), 265-302.

Nagata, N. (2002). BANZAI: An application of natural language processing to web-based language learning. *CALICO Journal, 19*(3), 583-599.

Norton, B. (2013). *Identity and language learning: Extending the conversation* (2nd ed.). Multilingual Matters.

Ouyang, L., Wu, J., Jiang, X., Almeida, D., Wainwright, C., Mishkin, P., ... & Lowe, R. (2022). Training language models to follow instructions with human feedback. *Advances in Neural Information Processing Systems, 35*, 27730-27744.

Oxford, R. L. (1990). *Language learning strategies: What every teacher should know*. Newbury House.

Pienemann, M. (1998). *Language processing and second language development: Processability theory*. John Benjamins.

Pratap, V., Tjandra, A., Shi, B., Tober, P., Babu, A., Kunber, S., ... & Auli, M. (2024). Scaling speech technology to 1,000+ languages. *Journal of Machine Learning Research, 25*(97), 1-52.

Radford, A., Kim, J. W., Xu, T., Brockman, G., McLeavey, C., & Sutskever, I. (2023). Robust speech recognition via large-scale weak supervision. *Proceedings of the 40th International Conference on Machine Learning*, 28492-28518.

Schmidt, R. W. (1990). The role of consciousness in second language learning. *Applied Linguistics, 11*(2), 129-158.

Sennrich, R., Haddow, B., & Birch, A. (2016). Neural machine translation of rare words with subword units. *Proceedings of the 54th Annual Meeting of the Association for Computational Linguistics*, 1715-1725.

Settles, B., & Meeder, B. (2016). A trainable spaced repetition model for language learning. *Proceedings of the 54th Annual Meeting of the Association for Computational Linguistics*, 1848-1858.

Sharwood Smith, M. (1993). Input enhancement in instructed SLA: Theoretical bases. *Studies in Second Language Acquisition, 15*(2), 165-179.

Swain, M. (1995). Three functions of output in second language learning. In G. Cook & B. Seidlhofer (Eds.), *Principle and practice in applied linguistics* (pp. 125-144). Oxford University Press.

Taguchi, N., & Roever, C. (2017). *Second language pragmatics*. Oxford University Press.

Trahey, M., & White, L. (1993). Positive evidence and preemption in the second language classroom. *Studies in Second Language Acquisition, 15*(2), 181-204.

Vaswani, A., Shazeer, N., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A. N., ... & Polosukhin, I. (2017). Attention is all you need. *Advances in Neural Information Processing Systems, 30*, 5998-6008.

Warschauer, M. (1996). Computer-assisted language learning: An introduction. In S. Fotos (Ed.), *Multimedia language teaching* (pp. 3-20). Logos International.

Yan, D. (2023). Impact of ChatGPT on learners in a L2 writing practicum: An exploratory investigation. *Education and Information Technologies, 29*, 13163-13186.

Zhang, Y., Han, W., Bapna, A., Cherry, C., Heafield, K., & Wu, Y. (2023). Google USM: Scaling automatic speech recognition beyond 100 languages. *arXiv preprint arXiv:2303.01037*.
