# Chapter 8: Vocabulary Acquisition and AI

## From Flashcards to Contextual Intelligence

---

## 8.1 Introduction: The Oldest Problem, the Newest Tools

Vocabulary acquisition occupies a peculiar position in second language acquisition research: it is simultaneously the most practical concern of every language learner ("How do I learn more words?") and one of the most theoretically complex domains in the field. The deceptive simplicity of "learning a word" dissolves upon inspection into a web of interrelated knowledge dimensions -- form, meaning, use, collocation, register, connotation, morphological derivation, grammatical behavior, and pragmatic constraint -- that collectively define what it means to "know" a word (Nation, 2001; Schmitt, 2010). A learner who can recognize the written form of *ubiquitous* on a multiple-choice test but cannot produce it in spontaneous speech, does not know its collocational patterns (*ubiquitous presence* but not *ubiquitous existence*), and has no sense of its register (formal, not conversational) has, in a meaningful sense, not acquired the word at all. They have acquired a fragment of a word.

This multidimensional nature of word knowledge has been the central challenge for vocabulary instruction since the field's inception. How does a learner move from zero knowledge of a word to the rich, interconnected, automatized knowledge that characterizes proficient use? The research literature has established that this journey requires multiple, varied encounters with a word across different contexts and modalities, over extended periods of time, with both intentional study and incidental exposure playing complementary roles (Nation, 2001; Webb, 2007; Schmitt, 2008).

Artificial intelligence has intervened at every point in this journey. Spaced repetition systems (SRS), the earliest AI-adjacent technology for vocabulary learning, have been optimizing the timing of review encounters since the 1970s. Adaptive algorithms now personalize which words a learner studies, when they study them, and how they are tested. Large language models can generate contextually rich example sentences, create personalized vocabulary exercises, explain semantic nuances, and engage learners in extended conversations designed to provide multiple encounters with target items. Word embedding models -- the mathematical representations that LLMs use internally -- bear a striking and theoretically provocative resemblance to the distributional patterns that usage-based linguists argue underlie human lexical acquisition.

This chapter examines AI-assisted vocabulary acquisition through the lens of established SLA vocabulary research, evaluating whether and how AI tools operationalize the principles that the empirical literature has identified as essential for deep, durable word knowledge. It begins with Nation's framework for vocabulary knowledge as the theoretical anchor, examines spaced repetition and its AI optimization, explores contextual vocabulary learning through AI, investigates the theoretical implications of word embeddings and semantic networks, addresses specialized vocabulary domains, identifies the pragmatic and cultural limitations of AI vocabulary tools, and reviews the empirical evidence on AI-assisted vocabulary learning outcomes.

---

## 8.2 What Does It Mean to Know a Word? Nation's Framework

### 8.2.1 The Multidimensional Nature of Lexical Knowledge

Nation's (2001) framework for word knowledge, refined across multiple editions of *Learning Vocabulary in Another Language*, provides the most comprehensive and widely cited description of what constitutes "knowing" a word. The framework distinguishes between three broad aspects of word knowledge -- form, meaning, and use -- each of which has receptive and productive dimensions.

**Form** encompasses spoken form (Can the learner recognize the word when heard? Can they pronounce it?), written form (Can they recognize it in print? Can they spell it?), and word parts (Can they recognize affixes and stems? Can they use word parts to create new forms?).

**Meaning** encompasses form-meaning connection (Can the learner recall the meaning when encountering the form? Can they produce the form when they want to express the meaning?), concept and referents (What does the word include in its meaning? What items can the concept refer to?), and associations (What other words does this word make the learner think of? What other words could they use instead?).

**Use** encompasses grammatical functions (In what patterns does the word occur? In what patterns can the learner use it?), collocations (What words or types of words occur with this one? What words or types of words must the learner use with it?), and constraints on use (Where, when, and how often would the learner expect to encounter this word? Where, when, and how often can the learner use it?).

This framework immediately reveals the poverty of most vocabulary assessment and, by extension, most AI vocabulary tools. A flashcard system that tests whether the learner can match "ubiquitous" to "present everywhere" is assessing exactly one cell in Nation's matrix: the receptive form-meaning connection. It tells us nothing about the learner's knowledge of pronunciation, spelling, collocational patterns, grammatical behavior, register constraints, or productive capability. Yet this single dimension -- receptive form-meaning matching -- is precisely what the vast majority of AI vocabulary tools measure and train.

### 8.2.2 Nation's Four Strands and Vocabulary Development

Nation (2007) also proposed that effective vocabulary programs should balance four "strands" of learning activity, each contributing approximately equally to instructional time:

1. **Meaning-focused input**: Learning vocabulary through reading and listening to comprehensible, interesting material. The learner encounters words in context, inferring meaning from surrounding text and gradually building form-meaning connections through repeated exposure.

2. **Meaning-focused output**: Learning vocabulary through speaking and writing activities where the learner needs to express meanings that push them to use new words productively. Swain's (1985) Output Hypothesis is relevant here: the act of producing language creates opportunities for noticing gaps in lexical knowledge.

3. **Language-focused learning**: Deliberate, intentional study of vocabulary items -- flashcards, word lists, dictionary work, vocabulary exercises. This strand provides the explicit, focused attention that many vocabulary items need to be initially noticed and learned.

4. **Fluency development**: Activities that help learners develop speed and automaticity with already-known vocabulary, moving words from slow, effortful retrieval to rapid, automatic access.

The four strands framework provides a useful lens for evaluating AI vocabulary tools. Most current AI applications concentrate heavily on the third strand (deliberate study), with some attention to the first (reading apps with vocabulary support). The second and fourth strands -- productive use and fluency development -- receive comparatively little AI attention, creating an imbalanced vocabulary learning ecology.

### 8.2.3 Vocabulary Size, Coverage, and the Threshold Problem

Research on vocabulary size thresholds has established that learners need approximately 8,000-9,000 word families for adequate comprehension of general written text and 6,000-7,000 word families for spoken text (Nation, 2006; Laufer & Ravenhorst-Kalovski, 2010). Below these thresholds, learners encounter too many unknown words for successful text comprehension, and reading/listening becomes an exercise in frustration rather than a source of incidental vocabulary growth.

These threshold findings have practical implications for AI vocabulary systems. A truly effective AI vocabulary program would need to help learners build not just random collections of "interesting" or "high-frequency" words but a strategically sequenced vocabulary that moves them toward coverage thresholds as efficiently as possible. This requires the AI to maintain a model of the learner's current vocabulary knowledge, compare it against frequency-based coverage targets, and prioritize items that will have the greatest marginal impact on the learner's ability to comprehend authentic text.

Some AI platforms have begun to implement this kind of strategic vocabulary building. Duolingo's Birdbrain system models individual vocabulary knowledge and sequences instruction accordingly. Lingvist uses statistical models to estimate vocabulary gaps and prioritize high-impact items. But the challenge is significant: estimating a learner's vocabulary knowledge with sufficient precision to make strategic recommendations requires far more data than most systems collect, and the relationship between word frequency and learnability is mediated by numerous factors (cognate status, concreteness, morphological transparency) that simple frequency lists do not capture.

---

## 8.3 Spaced Repetition and AI Optimization

### 8.3.1 The Science of Spacing

The spacing effect -- the finding that distributed practice produces better long-term retention than massed practice -- is one of the most robust phenomena in cognitive psychology, with a research history extending back to Ebbinghaus's (1885) pioneering self-experimentation with nonsense syllables. In the context of vocabulary learning, the spacing effect means that reviewing a word five times over five days produces substantially better retention than reviewing it five times in a single session, even though the total study time is identical.

The theoretical explanation for the spacing effect involves several complementary mechanisms. The retrieval practice account (Bjork & Bjork, 2011) holds that each successful retrieval from memory strengthens the memory trace, and that retrieval from longer delays produces stronger strengthening -- a principle Bjork (1994) termed "desirable difficulty." The encoding variability account (Raaijmakers, 2003) holds that spaced presentations occur in different cognitive contexts, providing more varied encoding cues that facilitate later retrieval. The consolidation account suggests that memories need time between activations to consolidate into long-term storage, and massed practice interferes with this consolidation process.

### 8.3.2 From Leitner to SM-2 to FSRS: The Algorithm Progression

Spaced repetition systems represent one of the earliest applications of algorithmic optimization to learning, predating the modern AI era by decades.

**Leitner's cardboard box system** (1972) was the first practical implementation of spaced repetition for vocabulary learning. Words are placed in one of several boxes; correctly recalled words move to the next box (which is reviewed less frequently), while forgotten words return to the first box (reviewed most frequently). Though entirely analog, the Leitner system embodies the key SRS principle: adapt review timing to individual item difficulty.

**SM-2** (SuperMemo algorithm version 2), developed by Piotr Wozniak in 1987, introduced computational optimization. SM-2 calculates the optimal interval between reviews based on item difficulty (estimated from the learner's recall history) and a global "easiness factor" that adjusts based on the learner's self-reported recall quality. SM-2 became the foundation for Anki, the most widely used open-source SRS platform, and its variants remain the backbone of many vocabulary learning applications.

**FSRS** (Free Spaced Repetition Scheduler), developed through a collaboration between machine learning researchers and the Anki community, represents the current state of the art. FSRS uses a more sophisticated mathematical model of memory -- incorporating the finding that memory stability increases with each successful retrieval and that the optimal review timing depends on the desired level of retention probability -- to calculate intervals that are empirically more efficient than SM-2. Anki integrated FSRS as its default scheduler in 2023, and initial research suggests 20-30% improvement in efficiency over SM-2 (Ye, 2023).

**Commercial SRS variants** in platforms like Memrise, Duolingo, Clozemaster, and Lingvist use proprietary algorithms that share the core SRS logic but incorporate additional signals: response time, error patterns, time of day, and (in some cases) collaborative filtering across the user base to estimate item difficulty from aggregate data rather than individual recall history alone.

### 8.3.3 The Strengths of SRS for Vocabulary

The evidence for SRS effectiveness in vocabulary learning is strong and consistent. Nakata (2015) conducted a comprehensive review of spacing research in L2 vocabulary acquisition and found robust advantages for spaced over massed practice across multiple studies, with effect sizes ranging from d = 0.50 to d = 1.20. Importantly, the spacing advantage was found for both receptive and productive knowledge, though the effect was stronger for receptive (recognition) than productive (recall) knowledge.

Kornell (2009) demonstrated that even learners who perceive massed practice as more effective actually learn better with spaced practice -- a metacognitive illusion that helps explain why many learners resist SRS despite its empirical superiority. The implication for AI vocabulary tools is that effectiveness and user preference may diverge, and that system design must sometimes override learner intuition in scheduling reviews.

### 8.3.4 The Limitations of SRS for Vocabulary

Despite its effectiveness for the form-meaning connection, SRS has well-documented limitations that map onto the gaps in Nation's vocabulary knowledge framework.

**Depth of processing**: The typical SRS interaction -- see a cue, retrieve a response, evaluate success -- involves relatively shallow processing. Craik and Lockhart's (1972) Depth of Processing framework predicts that deeper, more elaborative processing leads to better retention. While retrieving a word from memory does constitute deeper processing than merely re-reading it (the testing effect; Roediger & Karpicke, 2006), the repetitive, decontextualized nature of flashcard review limits the depth of semantic processing compared to encountering a word in a rich communicative context.

**Contextual poverty**: SRS reviews typically present words in isolation or with minimal context (a single example sentence). This decontextualization limits the development of collocational knowledge, register awareness, and pragmatic competence -- precisely the "use" dimensions of Nation's framework. A learner who has memorized that *arduous* means "difficult and tiring" through SRS may not know that we say *arduous journey* but not *arduous homework*, or that the word belongs to formal written English rather than casual conversation.

**Productive knowledge**: Most SRS interactions test receptive knowledge (L2 form to L1 meaning) rather than productive knowledge (L1 meaning to L2 form). While some systems include productive cards, the asymmetry is pronounced. Webb (2009) demonstrated that receptive and productive vocabulary knowledge develop at different rates and require different types of practice, suggesting that SRS optimized for receptive knowledge may not optimally support productive development.

**Motivation and engagement**: SRS requires sustained, daily practice over months and years to be effective. The repetitive nature of flashcard review, even when algorithmically optimized, leads to high attrition rates. Loewen et al. (2019) found that many learners who begin using SRS abandon it within weeks, often before the spacing algorithm has had time to demonstrate its effectiveness. This is a fundamental design challenge: the system that is most effective for long-term retention is also the system that many learners find too tedious to sustain.

---

## 8.4 Contextual Vocabulary Learning Through AI

### 8.4.1 Incidental Vocabulary Acquisition and AI-Enhanced Reading

One of the most robust findings in vocabulary acquisition research is that extensive reading -- reading large quantities of comprehensible text for meaning and pleasure -- produces significant incidental vocabulary growth (Waring & Takaki, 2003; Webb & Chang, 2015). The mechanism is straightforward: repeated encounters with unknown words in informative contexts allow learners to gradually infer and consolidate form-meaning connections. Krashen's (1989) argument that "reading is the only way we become good readers, develop a good writing style, an adequate vocabulary, advanced grammar, and the only way we become good spellers" reflects this perspective, even if it overstates the case.

The challenge with extensive reading for vocabulary acquisition is the vocabulary-threshold paradox: learners need approximately 95-98% text coverage (knowing 95-98% of the running words) to comprehend a text well enough to infer the meanings of unknown words (Hu & Nation, 2000; Laufer, 1989). Below this threshold, there are too many unknown words for successful inference, and reading becomes laborious rather than pleasurable.

AI can address this paradox in several ways:

**Text simplification**: AI systems can automatically simplify texts to match a learner's vocabulary level while preserving content and communicative authenticity. Crossley, Allen, and McNamara (2012) demonstrated that computational text simplification tools could reliably reduce vocabulary and syntactic complexity while maintaining meaning. LLM-based simplification has advanced considerably since then, with systems capable of rewriting texts at specified CEFR levels or vocabulary frequency bands while preserving the original's tone, style, and informational content.

**Glossing and pop-up definitions**: AI-powered reading apps (e.g., LingQ, Readlang, Lingua.com) provide instant definitions for unknown words when the learner taps or hovers over them. This "just-in-time" glossing reduces the cognitive load of reading with unknown words and has been shown to facilitate both text comprehension and vocabulary retention (Abraham, 2008; Yanagisawa, Webb, & Uchihara, 2020). However, the ease of accessing definitions may reduce the inferencing effort that some researchers argue promotes deeper processing (Hulstijn, 1992).

**Adaptive reading platforms**: Systems like Newsela and ReadWorks use AI to adjust text difficulty to individual learners, ensuring that each reader encounters texts at their optimal level of challenge -- enough unknown words to promote vocabulary growth but not so many as to impede comprehension. Duolingo's reading exercises similarly adapt vocabulary load to the learner's estimated proficiency.

### 8.4.2 The Involvement Load Hypothesis and AI Design

Laufer and Hulstijn's (2001) Involvement Load Hypothesis (ILH) provides a particularly useful framework for evaluating AI vocabulary tools because it specifies the cognitive conditions under which vocabulary processing is most effective. The hypothesis proposes three components of task-induced involvement:

**Need**: The motivational drive to process a word, which can be moderate (externally imposed, as when a teacher assigns a task) or strong (self-imposed, as when the learner looks up a word to express their own intended meaning).

**Search**: The effort to find the word's form or meaning, including dictionary lookup, contextual inference, or consultation with another person. Search requires active effort and is absent when the form or meaning is provided directly.

**Evaluation**: The comparison of a word with other words, or a specific meaning with other meanings, to determine whether the word fits a particular context. Evaluation requires decision-making about the appropriateness of a word choice.

Tasks with higher involvement loads (combining need, search, and evaluation) produce better vocabulary retention than tasks with lower involvement loads. This finding has been replicated across multiple studies (Keating, 2008; Kim, 2008; Hulstijn & Laufer, 2001).

The implications for AI vocabulary tool design are significant. Most AI vocabulary interactions minimize involvement load: the learner encounters a word, the AI provides the definition (eliminating search), and no evaluation is required because the correct answer is displayed rather than chosen. The efficiency of AI definition delivery -- which is its primary selling point -- directly undermines the cognitive conditions that the ILH identifies as most conducive to retention.

A well-designed AI vocabulary system would deliberately increase involvement load by:

- Requiring the learner to attempt contextual inference before revealing definitions (preserving search)
- Presenting multiple possible meanings and asking the learner to select the contextually appropriate one (inducing evaluation)
- Creating production tasks where the learner must use the target word to express their own meaning (generating need)
- Providing sentences with gaps where the learner must select from semantically similar alternatives (combining search and evaluation)

Some AI platforms have begun to implement these principles. Duolingo's sentence completion exercises induce evaluation by requiring learners to distinguish between semantically similar options. Clozemaster presents target words in authentic sentences with blanks, requiring the learner to produce the missing word from context. LLM-based vocabulary tutors can be designed to elicit word use in conversation before confirming or correcting the learner's usage. But these design choices are the exception rather than the rule in the current AI vocabulary landscape.

### 8.4.3 LLM-Generated Contexts and Vocabulary Learning

One of the most promising applications of LLMs for vocabulary learning is the generation of rich, varied, contextually appropriate example sentences and micro-texts that provide the multiple encounters research has identified as essential for deep word knowledge. Unlike pre-written dictionary examples, which are typically limited to one or two sentences per word, an LLM can generate dozens of contextually varied examples on demand, illustrating different meanings, collocational patterns, registers, and grammatical structures.

For instance, a learner studying the word *resilient* could request examples across contexts:

- Scientific: "The coral reef proved resilient to temperature fluctuations, recovering within a single season."
- Personal narrative: "After losing her job and her apartment in the same week, Maya discovered she was more resilient than she had ever imagined."
- Academic: "The resilient properties of the alloy made it suitable for aerospace applications requiring repeated stress cycles."
- Informal: "Kids are pretty resilient -- she was upset for about ten minutes and then went back to playing."

Each example illustrates the word in a different register, with different collocational patterns, revealing different facets of its meaning and use. This variety of contextual encounter is precisely what the vocabulary acquisition literature recommends (Webb, 2007; Schmitt, 2008) and what traditional learning materials rarely provide at scale.

However, the quality of LLM-generated examples is not guaranteed. LLMs can produce sentences that are grammatically correct but pragmatically unnatural, that illustrate atypical rather than prototypical uses of a word, or that contain subtle inaccuracies in collocation or register. The learner, who is by definition not yet proficient with the target word, is poorly positioned to evaluate the quality of the examples they receive. This creates a quality assurance challenge that is not yet adequately addressed by any current AI vocabulary platform.

---

## 8.5 Word Embeddings, Semantic Networks, and How LLMs "Know" Vocabulary

### 8.5.1 Distributional Semantics: The AI-Linguistics Connection

The theoretical foundation of LLM vocabulary knowledge is distributional semantics -- the hypothesis, attributed to Firth (1957) and Harris (1954), that the meaning of a word is determined by the contexts in which it occurs. Firth's famous dictum "You shall know a word by the company it keeps" is, in essence, the operating principle of every word embedding model and every large language model.

Word2vec (Mikolov et al., 2013) demonstrated that training a neural network to predict words from their contexts (or contexts from words) produces vector representations that capture remarkable semantic relationships. The now-famous example -- vec("king") - vec("man") + vec("woman") = vec("queen") -- illustrated that distributional patterns in text encode not just similarity but systematic relational structures.

Subsequent models -- GloVe (Pennington, Socher, & Manning, 2014), ELMo (Peters et al., 2018), and the transformer-based embeddings in BERT (Devlin et al., 2019) and GPT (Radford et al., 2018) -- have produced progressively richer representations. Critically, transformer-based models produce *contextual* embeddings: the representation of a word varies depending on its context, capturing polysemy in a way that static embeddings cannot. The word *bank* has a different vector representation in "river bank" than in "bank account" -- a distinction that human language users make effortlessly but that eluded computational models for decades.

### 8.5.2 The Usage-Based Parallel

The distributional semantics that underlies LLM vocabulary knowledge bears a striking resemblance to the usage-based theories of language acquisition advanced by Ellis (2002), Tomasello (2003), and others in the emergentist/connectionist tradition. Usage-based theories argue that language knowledge -- including vocabulary -- emerges from statistical regularities in the input: learners track the frequency and distribution of forms and gradually extract the patterns that constitute linguistic knowledge. Words are learned not as isolated form-meaning pairings but as components of larger patterns of co-occurrence that encode meaning, collocation, and grammatical behavior.

The parallel is provocative: LLMs and human learners may both acquire vocabulary through fundamentally similar statistical learning mechanisms, extracting meaning from distributional patterns in linguistic input. If this parallel holds, it suggests that the distributional information LLMs encode might align with the kind of vocabulary knowledge that human learners need -- not just form-meaning connections but the richer network of collocational, associative, and contextual relationships that constitute deep lexical knowledge.

However, the parallel has important limits. Human vocabulary acquisition is grounded in embodied, sensory, social experience in ways that LLM "acquisition" is not. When a child learns the word *hot*, they learn it in the context of touching a stove, hearing a caregiver's warning, and experiencing the sensation of heat. The word's meaning is anchored in a rich, multimodal, socially situated experience. When an LLM "learns" *hot*, it learns statistical associations between the string "hot" and other strings in its training data. The distributional patterns may be similar, but the underlying representations are fundamentally different in kind.

This distinction matters for vocabulary pedagogy because the aspects of word knowledge that distributional statistics capture well -- semantic similarity, collocation, typical syntactic patterns -- are not the same as the aspects that learners find most challenging. Pragmatic appropriateness, connotative nuance, cultural association, and the affective dimensions of word choice are precisely the areas where distributional statistics are weakest and where embodied, social experience is most important.

### 8.5.3 Implications for AI Vocabulary Tools

The distributional semantics foundation of LLMs creates both opportunities and limitations for AI vocabulary tools.

**Opportunities**: LLMs can leverage their distributional knowledge to provide learners with collocational information ("Words commonly used with *resilient* include *community*, *spirit*, *economy*, *ecosystem*"), register information ("*resilient* is used in both formal and informal contexts, but *tenacious* is more formal"), and associative networks ("Related words include *durable*, *robust*, *persistent*, *hardy*, each with slightly different connotations"). This kind of rich lexical information, which is difficult to find in traditional dictionaries and impossible to derive from flashcards, represents a genuine advance in AI-assisted vocabulary learning.

**Limitations**: LLMs cannot provide the embodied, experiential grounding that anchors word knowledge in human cognition. They cannot explain why *home* feels warm while *domicile* feels cold, why *cheap* is pejorative while *inexpensive* is neutral, or why *terrorist* and *freedom fighter* can refer to the same person. These distinctions require cultural knowledge, social experience, and affective sensitivity that distributional statistics approximate but do not capture.

---

## 8.6 AI for Specialized and Academic Vocabulary

### 8.6.1 The Academic Word List and Beyond

Coxhead's (2000) Academic Word List (AWL) identified 570 word families that occur frequently across academic disciplines but are not among the most frequent 2,000 general English word families. Knowledge of the AWL, combined with the first 2,000 general frequency words, provides approximately 90% coverage of academic text -- a significant boost toward the comprehension threshold. Subsequent research has produced more refined lists, including Cobb and Horst's (2015) analysis of discipline-specific vocabulary and Gardner and Davies' (2014) Academic Vocabulary List based on the Corpus of Contemporary American English.

AI offers powerful tools for specialized vocabulary instruction because it can analyze the specific texts a learner will encounter and generate vocabulary instruction tailored to those texts. An LLM can:

- Analyze a course reading list and identify the high-frequency academic vocabulary items the learner will need
- Compare a learner's current vocabulary knowledge (assessed through brief diagnostic testing) against the vocabulary demands of their target texts
- Generate discipline-specific example sentences that illustrate academic words in the learner's field of study
- Create vocabulary exercises that use authentic academic language from the learner's discipline
- Provide metalinguistic explanation of word formation patterns (affixes, roots) common in academic English

This kind of personalized, discipline-specific vocabulary instruction was previously available only through individual tutoring. AI makes it scalable.

### 8.6.2 Technical Vocabulary and Domain-Specific Corpora

For learners in specialized professional or academic contexts -- medical students learning clinical terminology, law students learning legal English, engineering students learning technical specifications -- AI offers particular advantages. LLMs trained on domain-specific corpora can provide not just definitions but contextually grounded explanations of how technical terms function in their fields. They can distinguish between the everyday meaning of a word and its technical meaning (*stress* in physics vs. psychology vs. common usage), explain field-specific collocational patterns (*administer medication* but *prescribe medication*), and generate practice scenarios that simulate the professional contexts in which the vocabulary will be used.

Nation (2001) distinguished between high-frequency vocabulary (the first 2,000 word families, useful across all contexts), academic vocabulary (useful across academic disciplines), and technical vocabulary (useful within a specific discipline). AI's capacity to work across all three levels -- and to sequence instruction from high-frequency through academic to technical -- represents a genuine advance over one-size-fits-all vocabulary programs.

### 8.6.3 The Multiword Unit Challenge

Research on formulaic language -- collocations, idioms, phrasal verbs, lexical bundles -- has established that proficient language use depends not just on knowledge of individual words but on knowledge of multiword units that function as single meaning-bearing chunks (Wray, 2002; Biber & Barbieri, 2007). Formulaic language is pervasive in both spoken and written discourse: Erman and Warren (2000) estimated that formulaic sequences constitute approximately 55% of running text.

AI tools have historically struggled with multiword units because most vocabulary algorithms treat the "word" as the fundamental unit. Flashcard systems test individual words, not collocations. Frequency lists count word forms, not multi-word sequences. Adaptive algorithms model word-level knowledge, not phrase-level knowledge.

LLMs represent a significant advance in this domain because their distributional training naturally captures multi-word patterns. An LLM "knows" that *take into account* functions as a unit, that *by and large* means "generally," and that *make a decision* and *take a decision* are regional variants. This knowledge can be leveraged for vocabulary instruction that moves beyond the single-word focus of traditional tools, teaching learners the chunks and formulaic sequences that are essential for fluent, natural production.

However, the explicit teaching of formulaic language through AI is still in its infancy. Most AI vocabulary tools remain word-focused, and the integration of multiword unit instruction into AI-powered vocabulary programs represents an important area for development.

---

## 8.7 Limitations: Pragmatic and Cultural Dimensions of Lexical Knowledge

### 8.7.1 Connotation, Affect, and Cultural Resonance

Words carry affective and cultural associations that go beyond their denotative meaning and that are poorly captured by distributional statistics. The word *thrifty* and the word *stingy* denote similar behaviors (spending little money) but carry opposite evaluative connotations. The word *homeland* carries different emotional weight in German, American English, and Palestinian Arabic. The word *comrade* has different associations in British English, Russian, and Chinese political discourse.

AI vocabulary tools, grounded in distributional semantics, tend to treat connotative and cultural meaning as secondary or peripheral to "core" meaning. A learner using an AI tool might learn that *slim*, *thin*, *skinny*, and *scrawny* are synonyms without understanding the evaluative gradient from positive (*slim*) through neutral (*thin*) to negative (*skinny*, *scrawny*). An LLM can explain these distinctions when explicitly asked, but the default behavior of most AI vocabulary tools is to present synonyms as interchangeable, obscuring the connotative nuances that are essential for appropriate word choice.

### 8.7.2 Pragmatic Competence and Word Choice

Vocabulary knowledge in its fullest sense includes knowing when to use a word and when not to -- the pragmatic dimension that Nation (2001) captured under "constraints on use." A proficient speaker of English knows that *deceased* is appropriate in formal contexts but odd in casual conversation ("My grandmother is deceased" vs. "My grandmother died/passed away"), that *fire* is more common than *terminate* in everyday workplace English, and that *awesome* in its contemporary colloquial sense is restricted to informal registers.

AI vocabulary tools struggle with pragmatic instruction for several reasons. First, pragmatic knowledge is context-dependent in ways that are difficult to encode in vocabulary learning exercises. The appropriateness of a word depends on the relationship between the speakers, the formality of the situation, the cultural context, and the communicative purpose -- variables that are typically absent from decontextualized vocabulary study. Second, LLMs have been trained on a mixture of registers and styles, making it difficult for them to consistently model a single register or to provide reliable pragmatic guidance about register appropriateness. Third, pragmatic norms vary across varieties of English and across cultures, and AI systems trained predominantly on American English data may provide guidance that is inappropriate for learners targeting other varieties.

### 8.7.3 The Monocultural Bias in AI Vocabulary

The training data for most LLMs is disproportionately English-language, and within English, disproportionately American. This creates a systematic bias in vocabulary instruction that privileges American English norms, American cultural references, and American pragmatic conventions. A learner in Japan studying English through an LLM-based vocabulary tool receives vocabulary instruction filtered through American distributional patterns, even if their target variety is British English, Indian English, or international English.

This bias extends beyond variety-specific vocabulary differences (e.g., *lorry* vs. *truck*, *flat* vs. *apartment*) to deeper cultural assumptions about what words mean and how they are used. The word *success*, for instance, has different prototypical associations in individualistic and collectivistic cultures. The word *family* encompasses different constellations of relationships across cultures. An AI vocabulary tool that defines *family* as "parents and their children" reflects a nuclear family norm that is culturally specific rather than universal.

For learners of languages other than English, the bias is even more pronounced. AI tools for less-resourced languages have smaller training corpora, less sophisticated models, and less reliable vocabulary knowledge. A learner of Swahili, Vietnamese, or Quechua using AI vocabulary tools will receive substantially less accurate and less comprehensive support than a learner of English, Spanish, or French, reinforcing existing inequities in language education access.

---

## 8.8 Research Evidence on AI-Assisted Vocabulary Learning

### 8.8.1 SRS Effectiveness Studies

The empirical evidence on spaced repetition for L2 vocabulary is among the strongest in the CALL literature. Nakata and Webb (2016) conducted a comprehensive review and found consistent advantages for spaced over massed practice, with larger spacing intervals generally producing better long-term retention (though with diminishing returns beyond certain intervals). Importantly, they found that the spacing effect held across different test types (recognition, recall, productive use), different language pairs, and different proficiency levels.

Studies specifically examining AI-optimized SRS have produced encouraging results. Settles and Meeder (2016), in a large-scale study of Duolingo users, found that spaced repetition scheduling based on a half-life regression model significantly improved vocabulary retention compared to fixed schedules. Ye (2023) reported that FSRS-scheduled reviews in Anki produced higher retention rates with fewer reviews than the SM-2 algorithm, suggesting that algorithmic improvements translate into real learning gains.

However, these studies typically measure form-meaning connection (receptive vocabulary knowledge) and rarely assess depth of knowledge, productive ability, or transfer to communicative contexts. The question of whether SRS-acquired vocabulary transfers to reading comprehension, speaking fluency, or writing quality remains underexplored.

### 8.8.2 AI-Enhanced Reading and Incidental Vocabulary Growth

Studies of AI-enhanced reading environments have generally found positive effects on vocabulary learning, though with important qualifications. Abraham (2008) conducted a meta-analysis of computer-mediated glossing studies and found a medium effect size (d = 0.73) for glossed over non-glossed reading conditions on vocabulary posttests. Yanagisawa et al. (2020) updated this meta-analysis with more recent studies and confirmed the positive effect, while noting that glossing effects were stronger for receptive than productive vocabulary knowledge and that multimedia glosses (text + image + audio) outperformed text-only glosses.

AI-specific enhancements to reading environments -- adaptive text difficulty, personalized vocabulary selection, contextual recommendations -- have shown promise but have been less extensively studied. Ma and Kelly (2006) found that a computer-based extensive reading program with vocabulary support produced significant vocabulary gains, and more recent studies of platforms like LingQ (Loewen et al., 2019) and Readlang have reported positive user experiences, though controlled experimental evidence is limited.

### 8.8.3 LLM-Based Vocabulary Instruction

The use of LLMs for vocabulary instruction is a very recent phenomenon, and the research base is still thin. Early studies have been cautiously optimistic. Chen (2024) found that Chinese EFL learners who used ChatGPT for vocabulary exploration -- generating examples, asking about collocations, requesting explanations of nuance -- showed significant gains on vocabulary depth measures compared to a control group using traditional dictionary study. Importantly, the gains were not limited to form-meaning connection but extended to collocational knowledge and contextual use, suggesting that the interactive, exploratory nature of LLM-based vocabulary study promotes the kind of deep processing that traditional tools do not.

Baskara (2023) reported that Indonesian EFL learners found LLM-based vocabulary instruction more engaging and more informative than traditional methods, particularly for learning collocations and register distinctions. However, the study also found that learners had difficulty evaluating the accuracy of LLM-generated examples and sometimes internalized incorrect collocational patterns from AI output.

These findings point to both the promise and the peril of LLM-based vocabulary instruction: the technology can provide the rich, contextually varied, interactive encounters that vocabulary research recommends, but only if the quality of its output is reliable and if learners develop the critical literacy to evaluate AI-generated language.

### 8.8.4 Comparative Studies: AI vs. Human Vocabulary Instruction

Direct comparisons between AI-assisted and human-led vocabulary instruction are surprisingly rare, given the practical importance of the question. The studies that exist suggest approximate parity for form-meaning learning, with advantages for human instruction on deeper dimensions of word knowledge.

Wilkinson (2016) compared vocabulary gains in learners using a computer-based adaptive vocabulary program versus learners receiving classroom vocabulary instruction and found no significant difference on delayed receptive vocabulary tests but significantly better performance for the classroom group on productive use measures. This pattern -- AI comparable for receptive knowledge, human instruction superior for productive knowledge -- has been replicated in several subsequent studies and aligns with the theoretical analysis presented throughout this chapter: AI tools optimize for the dimensions of vocabulary knowledge they can measure (form-meaning connection) while underserving the dimensions they cannot (productive use, pragmatic competence, social register).

---

## 8.9 Designing AI Vocabulary Systems: Principles from SLA Research

### 8.9.1 Operationalizing Nation's Four Strands in AI

An AI vocabulary system designed according to SLA principles would balance all four of Nation's strands rather than concentrating on deliberate study:

**Meaning-focused input**: AI-enhanced extensive reading and listening platforms that adapt vocabulary load to the learner's level, provide just-in-time glossing calibrated to minimize interference with comprehension processing, and track incidental vocabulary encounters to inform the deliberate study strand.

**Meaning-focused output**: LLM-based conversational and writing activities designed to push learners to use newly encountered vocabulary productively. The AI would create communicative tasks that require the use of specific target items without making the task feel like a vocabulary drill -- for example, asking the learner to write a paragraph arguing for or against a proposition, where the relevant vocabulary is needed to express the argument effectively.

**Deliberate study**: SRS optimized not just for form-meaning connection but for the full range of Nation's knowledge dimensions. This would include collocational study (what words typically co-occur with the target item?), receptive and productive testing in alternation, context-varied review (presenting the word in different sentence contexts on each review), and metalinguistic study of word parts and derivational patterns.

**Fluency development**: Speed-focused activities using already-known vocabulary -- timed reading, rapid word association, speed-writing prompts -- designed to move words from effortful retrieval to automatic access. AI can personalize fluency activities based on which words the learner knows but still processes slowly.

### 8.9.2 Increasing Involvement Load in AI Vocabulary Tools

Following Laufer and Hulstijn's (2001) Involvement Load Hypothesis, AI vocabulary tools should be designed to maximize cognitive involvement:

**Inducing need**: Create tasks where the learner discovers they need a word to express their intended meaning, rather than presenting words for study in isolation. An LLM-based writing tutor could assign a topic, let the learner write, identify vocabulary gaps in the learner's production, and then teach the needed words -- reversing the typical sequence of "learn words first, then use them."

**Preserving search**: Instead of providing definitions immediately, require the learner to attempt inference from context, look up words in a dictionary, or ask the AI tutor questions -- any process that involves active effort to determine meaning.

**Requiring evaluation**: Present vocabulary items in contexts that require the learner to make decisions about appropriateness, register, and collocation. "Which sentence sounds more natural: 'She made a big mistake' or 'She committed a big mistake'?" requires evaluation that simple definition retrieval does not.

### 8.9.3 Addressing the Productive Knowledge Gap

The most significant limitation of current AI vocabulary tools -- their focus on receptive at the expense of productive knowledge -- can be addressed through deliberate design:

**Productive SRS**: Include L1-to-L2 production cards in SRS alongside the more common L2-to-L1 recognition cards. FSRS and other modern algorithms can schedule these separately, recognizing that the same word may require different intervals for receptive versus productive review.

**Sentence production tasks**: Rather than testing vocabulary through recognition or cloze exercises, require learners to produce original sentences using target words. LLMs can evaluate the accuracy and appropriateness of learner-produced sentences, providing feedback on whether the word has been used correctly in context.

**Conversation-based vocabulary practice**: LLM-based conversation partners can be designed to create communicative contexts that require the learner to produce target vocabulary items. Unlike scripted dialogue exercises, LLM conversations can adapt to the learner's responses, providing a more authentic productive vocabulary practice environment.

---

## 8.10 The Future of AI-Assisted Vocabulary Learning

### 8.10.1 Multimodal Vocabulary Learning

Emerging AI capabilities in image generation, video synthesis, and speech processing open new possibilities for vocabulary instruction that engages multiple modalities. Paivio's (1986) Dual Coding Theory and Mayer's (2009) Cognitive Theory of Multimedia Learning both predict that vocabulary items encoded through both verbal and visual channels will be retained better than items encoded through a single channel. AI systems that can generate contextually appropriate images for vocabulary items, produce audio examples in natural speech, and create short video scenarios illustrating word use in context would provide the multimodal input that vocabulary research recommends.

### 8.10.2 Personalized Vocabulary Trajectories

The next frontier in AI vocabulary instruction is the move from item-level personalization (scheduling individual word reviews based on recall history) to trajectory-level personalization (designing an individualized vocabulary learning pathway based on the learner's goals, current knowledge, target contexts, and learning preferences). This would require AI systems that can:

- Assess current vocabulary knowledge comprehensively, including depth and productive ability
- Model the vocabulary demands of the learner's target communicative contexts
- Identify the vocabulary items that will have the greatest marginal impact on the learner's communicative ability
- Sequence instruction across Nation's four strands, balancing incidental and intentional learning
- Adapt the trajectory based on ongoing assessment of learning outcomes

Such a system would represent a qualitative advance over current AI vocabulary tools, which optimize locally (scheduling the next review of a specific item) without optimizing globally (planning the learner's overall vocabulary development trajectory).

### 8.10.3 Corpus-Informed, AI-Delivered Instruction

The integration of corpus linguistics tools with AI delivery systems offers a powerful combination for vocabulary instruction. AI can analyze authentic corpora to identify the most frequent and useful collocations, the most common grammatical patterns, and the most typical contextual frames for a given word, and then present this information to learners in accessible, pedagogically organized formats. This "corpus-informed, AI-delivered" approach combines the empirical rigor of corpus research with the accessibility and personalization of AI instruction.

---

## 8.11 Conclusion

Vocabulary acquisition sits at the intersection of what AI does best (pattern recognition, personalization, scale) and what it struggles with most (pragmatic nuance, cultural sensitivity, experiential grounding). The SRS algorithms that power flashcard apps represent one of the most empirically validated applications of adaptive technology in education, reliably improving the form-meaning connections that are the foundation of vocabulary knowledge. LLMs offer genuinely new possibilities for contextual, interactive vocabulary learning that moves beyond the flashcard paradigm toward the rich, multi-encounter, multi-dimensional word knowledge that Nation's framework describes.

Yet the analysis in this chapter reveals persistent gaps between what vocabulary acquisition research recommends and what AI vocabulary tools provide. The dominance of receptive over productive practice, the shallow processing encouraged by instant definitions, the decontextualization of SRS review, the pragmatic and cultural blind spots of distributional semantics, and the monocultural bias of English-centric training data all represent areas where current AI tools fall short of the principles established by decades of vocabulary research.

The path forward requires AI vocabulary tools designed by people who understand both the technology and the research -- tools that deliberately increase involvement load rather than minimizing user effort, that balance all four of Nation's strands rather than concentrating on deliberate study, that develop productive as well as receptive knowledge, and that address the pragmatic, cultural, and register dimensions of word knowledge that distributional statistics alone cannot capture.

The flashcard is not dead, but it was never enough. The question is whether AI can deliver the something more that vocabulary acquisition demands.

---

## References

Abraham, L. B. (2008). Computer-mediated glosses in second language reading comprehension and vocabulary learning: A meta-analysis. *Computer Assisted Language Learning*, 21(3), 199-226.

Baskara, F. R. (2023). ChatGPT as a virtual learning companion for EFL vocabulary acquisition. *Journal of English Language Teaching and Linguistics*, 8(2), 245-258.

Biber, D., & Barbieri, F. (2007). Lexical bundles in university spoken and written registers. *English for Specific Purposes*, 26(3), 263-286.

Bjork, R. A. (1994). Memory and metamemory considerations in the training of human beings. In J. Metcalfe & A. Shimamura (Eds.), *Metacognition: Knowing about knowing* (pp. 185-205). MIT Press.

Bjork, E. L., & Bjork, R. A. (2011). Making things hard on yourself, but in a good way: Creating desirable difficulties to enhance learning. In M. A. Gernsbacher et al. (Eds.), *Psychology and the real world* (pp. 56-64). Worth Publishers.

Chen, Y. (2024). Exploring ChatGPT-assisted vocabulary learning: Effects on vocabulary depth and breadth. *Computer Assisted Language Learning*, 37(4), 412-435.

Cobb, T., & Horst, M. (2015). Learner corpora and lexis. In S. Granger, G. Gilquin, & F. Meunier (Eds.), *The Cambridge handbook of learner corpus research* (pp. 185-206). Cambridge University Press.

Coxhead, A. (2000). A new academic word list. *TESOL Quarterly*, 34(2), 213-238.

Craik, F. I. M., & Lockhart, R. S. (1972). Levels of processing: A framework for memory research. *Journal of Verbal Learning and Verbal Behavior*, 11(6), 671-684.

Crossley, S. A., Allen, D., & McNamara, D. S. (2012). Text simplification and comprehensible input: A case for an intuitive approach. *Language Teaching Research*, 16(1), 89-108.

Devlin, J., Chang, M., Lee, K., & Toutanova, K. (2019). BERT: Pre-training of deep bidirectional transformers for language understanding. In *Proceedings of NAACL-HLT* (pp. 4171-4186).

Ebbinghaus, H. (1885). *Uber das Gedachtnis: Untersuchungen zur experimentellen Psychologie*. Duncker & Humblot.

Ellis, N. C. (2002). Frequency effects in language processing: A review with implications for theories of implicit and explicit language acquisition. *Studies in Second Language Acquisition*, 24(2), 143-188.

Erman, B., & Warren, B. (2000). The idiom principle and the open choice principle. *Text*, 20(1), 29-62.

Firth, J. R. (1957). A synopsis of linguistic theory 1930-1955. In *Studies in linguistic analysis* (pp. 1-32). Blackwell.

Gardner, D., & Davies, M. (2014). A new Academic Vocabulary List. *Applied Linguistics*, 35(3), 305-327.

Harris, Z. S. (1954). Distributional structure. *Word*, 10(2-3), 146-162.

Hu, M., & Nation, I. S. P. (2000). Unknown vocabulary density and reading comprehension. *Reading in a Foreign Language*, 13(1), 403-430.

Hulstijn, J. H. (1992). Retention of inferred and given word meanings: Experiments in incidental vocabulary learning. In P. J. L. Arnaud & H. Bejoint (Eds.), *Vocabulary and applied linguistics* (pp. 113-125). Macmillan.

Hulstijn, J. H., & Laufer, B. (2001). Some empirical evidence for the Involvement Load Hypothesis in vocabulary acquisition. *Language Learning*, 51(3), 539-558.

Keating, G. D. (2008). Task effectiveness and word learning in a second language: The Involvement Load Hypothesis on trial. *Language Teaching Research*, 12(3), 365-386.

Kim, Y. (2008). The role of task-induced involvement and learner proficiency in L2 vocabulary acquisition. *Language Learning*, 58(2), 285-325.

Kornell, N. (2009). Optimising learning using flashcards: Spacing is more effective than cramming. *Applied Cognitive Psychology*, 23(9), 1297-1317.

Krashen, S. D. (1989). We acquire vocabulary and spelling by reading: Additional evidence for the Input Hypothesis. *The Modern Language Journal*, 73(4), 440-464.

Laufer, B. (1989). What percentage of text-lexis is essential for comprehension? In C. Lauren & M. Nordman (Eds.), *Special language: From humans thinking to thinking machines* (pp. 316-323). Multilingual Matters.

Laufer, B., & Hulstijn, J. H. (2001). Incidental vocabulary acquisition in a second language: The construct of task-induced involvement. *Applied Linguistics*, 22(1), 1-26.

Laufer, B., & Ravenhorst-Kalovski, G. C. (2010). Lexical threshold revisited: Lexical text coverage, learners' vocabulary size and reading comprehension. *Reading in a Foreign Language*, 22(1), 15-30.

Leitner, S. (1972). *So lernt man lernen*. Herder.

Loewen, S., Crowther, D., Isbell, D. R., Kim, K. M., Maloney, J., Miller, Z. F., & Raber, H. (2019). Mobile-assisted language learning: A Duolingo case study. *ReCALL*, 31(3), 293-311.

Ma, Q., & Kelly, P. (2006). Computer assisted vocabulary learning: Design and evaluation. *Computer Assisted Language Learning*, 19(1), 15-45.

Mayer, R. E. (2009). *Multimedia learning* (2nd ed.). Cambridge University Press.

Mikolov, T., Sutskever, I., Chen, K., Corrado, G. S., & Dean, J. (2013). Distributed representations of words and phrases and their compositionality. In *Advances in neural information processing systems* (pp. 3111-3119).

Nakata, T. (2015). Effects of expanding and equal spacing on second language vocabulary learning. *Studies in Second Language Acquisition*, 37(4), 677-711.

Nakata, T., & Webb, S. (2016). Does studying vocabulary in smaller sets increase learning? *Studies in Second Language Acquisition*, 38(3), 523-552.

Nation, I. S. P. (2001). *Learning vocabulary in another language*. Cambridge University Press.

Nation, I. S. P. (2006). How large a vocabulary is needed for reading and listening? *The Canadian Modern Language Review*, 63(1), 59-82.

Nation, I. S. P. (2007). The four strands. *International Journal of Innovation in Language Learning and Teaching*, 1(1), 2-13.

Paivio, A. (1986). *Mental representations: A dual coding approach*. Oxford University Press.

Pennington, J., Socher, R., & Manning, C. D. (2014). GloVe: Global vectors for word representation. In *Proceedings of EMNLP* (pp. 1532-1543).

Peters, M. E., Neumann, M., Iyyer, M., Gardner, M., Clark, C., Lee, K., & Zettlemoyer, L. (2018). Deep contextualized word representations. In *Proceedings of NAACL-HLT* (pp. 2227-2237).

Raaijmakers, J. G. W. (2003). Spacing and repetition effects in human memory: Application of the SAM model. *Cognitive Science*, 27(3), 431-452.

Radford, A., Narasimhan, K., Salimans, T., & Sutskever, I. (2018). *Improving language understanding by generative pre-training*. OpenAI.

Roediger, H. L., & Karpicke, J. D. (2006). Test-enhanced learning: Taking memory tests improves long-term retention. *Psychological Science*, 17(3), 249-255.

Schmitt, N. (2008). Instructed second language vocabulary learning. *Language Teaching Research*, 12(3), 329-363.

Schmitt, N. (2010). *Researching vocabulary: A vocabulary research manual*. Palgrave Macmillan.

Settles, B., & Meeder, B. (2016). A trainable spaced repetition model for language learning. In *Proceedings of ACL* (pp. 1848-1858).

Swain, M. (1985). Communicative competence: Some roles of comprehensible input and comprehensible output in its development. In S. Gass & C. Madden (Eds.), *Input in second language acquisition* (pp. 235-253). Newbury House.

Tomasello, M. (2003). *Constructing a language: A usage-based theory of language acquisition*. Harvard University Press.

Waring, R., & Takaki, M. (2003). At what rate do learners learn and retain new vocabulary from reading a graded reader? *Reading in a Foreign Language*, 15(2), 130-163.

Webb, S. (2007). The effects of repetition on vocabulary knowledge. *Applied Linguistics*, 28(1), 46-65.

Webb, S. (2009). The effects of receptive and productive learning of word pairs on vocabulary knowledge. *RELC Journal*, 40(3), 360-376.

Webb, S., & Chang, A. C. S. (2015). How does prior word knowledge affect vocabulary learning progress in an extensive reading program? *Studies in Second Language Acquisition*, 37(4), 651-675.

Wilkinson, M. (2016). Technology-enhanced vocabulary learning and recall: A comparison of computer-based and classroom approaches. *ReCALL*, 28(2), 223-240.

Wray, A. (2002). *Formulaic language and the lexicon*. Cambridge University Press.

Yanagisawa, A., Webb, S., & Uchihara, T. (2020). How do different forms of glossing contribute to L2 vocabulary learning from reading? A meta-regression analysis. *Studies in Second Language Acquisition*, 42(2), 411-438.

Ye, W. (2023). Open spaced repetition: An open-source, modern spaced repetition scheduler. *ArXiv preprint arXiv:2310.02898*.
