# Chapter 13: AI and Multilingualism — Beyond the Monolingual Bias

---

## 13.1 Introduction: The Multilingual Reality and the Monolingual Machine

The majority of the world's population is multilingual. Estimates consistently place the proportion of individuals who regularly use two or more languages at between fifty and seventy percent of the global population (Grosjean, 2010; Wei, 2008). Multilingualism is not the exception in human linguistic experience; it is the norm. Yet the artificial intelligence systems that increasingly mediate language learning, language use, and language assessment have been designed, trained, and evaluated primarily through a monolingual lens — and predominantly an English monolingual lens at that. This chapter examines the profound implications of this misalignment between the multilingual reality of human language users and the monolingual architecture of most AI language systems.

The significance of this inquiry extends well beyond questions of technical capability. How AI systems conceptualize, model, and respond to multilingual language use has direct consequences for the millions of language learners worldwide who bring rich, complex linguistic repertoires to their encounters with technology. When an AI writing assistant flags a learner's translanguaging as an "error," when a speech recognition system fails to process code-switched utterances, or when an automated assessment tool penalizes a heritage speaker's dialectal features, these are not merely technical failures. They are ideological acts — instantiations of a monolingual ideology that decades of applied linguistics scholarship has worked to dismantle (Canagarajah, 2013; Garcia & Wei, 2014; Ortega, 2014).

This chapter draws on contemporary theories of multilingualism, translanguaging, and multi-competence to critically evaluate how AI systems interact with multilingual users and multilingual practices. It examines the technical foundations of AI's monolingual bias, explores how specific AI capabilities — machine translation, speech recognition, text generation, and language assessment — handle multilingual input, and proposes principles for designing AI systems that honor rather than suppress multilingual repertoires. Throughout, the discussion is grounded in the recognition that second language acquisition does not occur in a linguistic vacuum; every L2 learner is, by definition, becoming multilingual, and AI systems that fail to account for this fact are fundamentally misaligned with the populations they purport to serve.

---

## 13.2 Theoretical Foundations: Multi-competence, Translanguaging, and Dynamic Bilingualism

### 13.2.1 Cook's Multi-competence and the Rejection of the Monolingual Norm

The theoretical foundation for understanding multilingualism in the AI age begins with Vivian Cook's (1991, 2001, 2016) concept of multi-competence. Cook defined multi-competence as "the compound state of a mind with two grammars" (1991, p. 112), later expanding this to "the overall system of a mind or a community that uses more than one language" (2016, p. 2). The critical insight of multi-competence theory is that the multilingual mind is not two monolingual minds housed in a single skull. Rather, the languages of a multilingual individual form an integrated system that differs qualitatively from the linguistic system of a monolingual speaker of either language.

This reconceptualization has profound implications for AI design. Most AI language models are trained on monolingual corpora, evaluated against monolingual benchmarks, and deployed with the implicit assumption that competent language use means monolingual-like language use in a single language at a time. The multi-competence framework challenges this assumption at its root. If the multilingual mind constitutes a unified system rather than two separable monolingualisms, then AI systems designed to interact with multilingual users must be capable of engaging with this integrated system — including its characteristic patterns of cross-linguistic influence, code-switching, and translanguaging that are not deficiencies to be corrected but natural expressions of multi-competent language use.

Cook (2001) further argued that the native speaker should not serve as the benchmark for L2 learner achievement, a position with direct relevance to AI assessment systems. When automated scoring engines penalize syntactic structures or lexical choices that reflect cross-linguistic influence, they instantiate precisely the monolingual comparison that Cook identified as theoretically untenable. The L2 user is a legitimate language user in their own right, not a defective approximation of a monolingual native speaker (Cook, 2001; Ortega, 2014).

### 13.2.2 Garcia and Wei's Translanguaging Theory

The concept of translanguaging, as developed by Ofelia Garcia and Li Wei (2014), represents perhaps the most significant reconceptualization of multilingual practice in contemporary applied linguistics. Translanguaging refers to "the deployment of a speaker's full linguistic repertoire without regard for watchful adherence to the socially and politically defined boundaries of named languages" (Otheguy, Garcia, & Reid, 2015, p. 281). Under this view, multilingual speakers do not possess discrete, separable language systems (e.g., "their Spanish" and "their English") but rather a single integrated linguistic repertoire from which they draw resources as communicative contexts demand.

Garcia and Wei (2014) distinguished translanguaging from earlier concepts such as code-switching and code-mixing. While code-switching implies the alternation between two identifiable language systems — presupposing their separateness — translanguaging rejects the premise that named languages are discrete cognitive entities. Instead, translanguaging positions multilingual practice as the deployment of semiotic resources from a unified repertoire, with "named languages" being social and political constructs rather than cognitive realities.

For AI systems, the implications are significant. Consider an AI chatbot designed for Spanish language practice. A heritage speaker of Spanish who grew up in Los Angeles might produce utterances such as "Vamos al store porque necesito comprar unas cosas para la party de mi prima" — a perfectly natural translanguaging utterance that integrates English lexical items within a Spanish morphosyntactic frame. Most AI language learning systems would flag this as erroneous, offering corrections to replace the English words with Spanish equivalents. From a translanguaging perspective, however, this utterance represents competent multilingual practice — the strategic deployment of the speaker's full repertoire in a manner consistent with their community's communicative norms.

The challenge for AI design is not merely technical but ideological. Building AI systems that recognize and respond appropriately to translanguaging requires abandoning the monolingual frame that has governed both NLP engineering and much of SLA pedagogy. It requires, in Garcia and Wei's terms, designing for "dynamic bilingualism" rather than "additive bilingualism" — systems that support the development of an integrated multilingual repertoire rather than the accumulation of discrete monolingual-like competencies.

### 13.2.3 Cenoz and Gorter's Focus on Multilingualism

Cenoz and Gorter (2015) extended the translanguaging framework to educational contexts, arguing for a "Focus on Multilingualism" approach that recognizes three key principles: (a) the multilingual speaker is qualitatively different from the monolingual speaker, (b) the whole linguistic repertoire is available for communication and learning, and (c) multilingual practices such as translanguaging and code-switching serve cognitive and communicative functions that support learning.

Their work is particularly relevant to AI-mediated language learning because it challenges the common practice of enforcing monolingual interaction in the target language. Many AI tutoring systems are designed to conduct interactions exclusively in the target language, discouraging or penalizing L1 use. Cenoz and Gorter's framework suggests that strategic use of the full linguistic repertoire — including the L1 and any other languages the learner knows — can facilitate comprehension, metalinguistic awareness, and deeper processing. AI systems that artificially constrain learners to a single language may inadvertently reduce the cognitive resources available for learning.

### 13.2.4 Canagarajah's Translingual Practice

Suresh Canagarajah (2013) introduced the concept of "translingual practice" to capture the communicative competence involved in negotiating diverse linguistic resources in contexts of global mobility. Canagarajah argued that effective communication in multilingual settings depends not on mastery of discrete languages but on the ability to shuttle between language varieties, negotiate meaning across difference, and co-construct understanding through adaptive, creative language use.

This perspective has particular relevance for AI-mediated communication. As AI systems increasingly serve as mediators in cross-linguistic communication — through machine translation, multilingual chatbots, and AI-assisted writing tools — their capacity to support translingual practice becomes critical. An AI writing assistant that helps a multilingual scholar negotiate between the conventions of academic English and the rhetorical patterns of their L1 academic tradition is engaging in a fundamentally different task than one that simply "corrects" non-standard English. The former supports translingual competence; the latter suppresses it.

---

## 13.3 The Monolingual Bias in AI: Technical Foundations and Ideological Implications

### 13.3.1 Training Data and the English Hegemony

The monolingual bias in AI language systems begins at the level of training data. Large language models (LLMs) such as GPT-4, Claude, and Gemini are trained on massive corpora that are overwhelmingly dominated by English text. Common Crawl, the web scraping dataset that forms the backbone of many LLM training sets, contains approximately 46% English content, followed by Russian, German, Japanese, and French at roughly 5-6% each (Dodge et al., 2021). Languages such as Yoruba, Quechua, Tagalog, Swahili, and the vast majority of the world's approximately 7,000 languages are minimally represented or entirely absent.

This distributional imbalance has cascading consequences. Models trained predominantly on English develop stronger capabilities in English — better grammar, more nuanced vocabulary, more contextually appropriate responses — and progressively weaker capabilities in lower-resourced languages. Joshi et al. (2020) classified the world's languages into six categories based on digital resource availability, from "the winners" (primarily English, along with major European and East Asian languages) through "the left-behinds" (roughly 88% of the world's languages for which virtually no NLP resources exist). AI systems built on these skewed foundations inevitably reproduce and amplify existing linguistic inequalities.

The implications for SLA are direct. A learner of Amharic using an AI chatbot will receive qualitatively inferior interaction compared to a learner of English. The AI's responses will be less fluent, less nuanced, less culturally appropriate, and more prone to grammatical errors in Amharic than in English. When these same AI systems are used for language assessment, the differential in system capability translates directly into differential measurement validity — a fairness concern of the first order.

### 13.3.2 Tokenization and Morphological Bias

The monolingual bias extends to the technical architecture of language models. Tokenization — the process by which text is broken into sub-word units for model processing — is typically optimized for English and other analytic languages. The byte-pair encoding (BPE) algorithm widely used in transformer models (Sennrich, Haddow, & Birch, 2016) creates a vocabulary of sub-word tokens based on the frequency distribution of character sequences in the training data. Because English dominates the training corpus, English words tend to be represented by fewer tokens (often a single token per common word), while words in lower-resourced or morphologically complex languages may be fragmented into many tokens.

This asymmetry has practical consequences. A Turkish word such as "evlerinizden" (from your houses) might be tokenized into four or five sub-word units, while the equivalent English phrase "from your houses" uses three common single-word tokens. The model must process more tokens for the same semantic content in Turkish, consuming more of its context window and potentially degrading performance. For agglutinative languages such as Turkish, Finnish, Korean, and many indigenous languages of the Americas, this tokenization penalty is substantial and systematic.

For language learners, the tokenization issue manifests as degraded AI performance precisely in the languages where learners most need support. Learners studying agglutinative or polysynthetic languages through AI tools will encounter more errors, less natural output, and less effective feedback than learners studying analytically simpler languages — not because these languages are inherently more difficult for AI but because the technical infrastructure was designed with English-like languages in mind.

### 13.3.3 Evaluation Metrics and Monolingual Benchmarks

The evaluation of AI language systems further entrenches monolingual norms. Standard NLP benchmarks — GLUE, SuperGLUE, HellaSwag, MMLU, and their successors — are predominantly English-language tasks. While multilingual benchmarks exist (XTREME, XGLUE, MEGA), they typically evaluate performance in individual languages independently rather than assessing multilingual competence as an integrated phenomenon (Ruder et al., 2021). There is no standard benchmark for evaluating how well a language model handles code-switched input, translanguaged discourse, or multilingual conversation that flows naturally between languages.

This evaluation gap means that the AI community literally does not measure the capabilities that matter most for multilingual users. Model developers can claim "multilingual capability" based on performance in individual languages while their systems systematically fail on the mixed-language input that characterizes actual multilingual communication. For language learners whose natural communication patterns include code-switching and translanguaging, this evaluation blindspot translates directly into degraded user experience.

### 13.3.4 Named Languages as Ideological Constructs in AI Architecture

At the deepest level, the monolingual bias in AI reflects an ideological commitment to named languages as natural, discrete categories — precisely the assumption that translanguaging theory challenges. AI systems are built around language identification, language selection, and language-specific processing. A user must typically select a language before interacting with a chatbot, a translation system, or a text-to-speech engine. The system then processes input and generates output within the bounds of that selected language.

This architecture mirrors what Makoni and Pennycook (2007) called the "invention of languages" — the historical process by which continuous spectra of linguistic practice were divided into discrete, named, bounded entities through colonial, nationalist, and institutional processes. When AI systems require users to operate within a single named language at a time, they instantiate a particular ideology of language that much of contemporary sociolinguistics has rejected. The technical architecture is not ideologically neutral; it encodes assumptions about what language is and how it should be used.

---

## 13.4 Machine Translation and Multilingual Practice

### 13.4.1 From Threat to Tool: The Evolving View of MT in SLA

Machine translation (MT) has long been viewed with suspicion in language education. Teachers have warned students against using Google Translate, treating MT as a form of cheating that circumvents the cognitive work necessary for acquisition. This prohibition rests on the implicit assumption that language learning requires unmediated engagement with the target language — an assumption rooted in the monolingual target language norm that translanguaging theory questions.

Recent scholarship has begun to reconceptualize MT as a potentially valuable pedagogical tool rather than an obstacle to learning. Gonzalez-Davies (2004, 2014) argued persuasively that translation activities — long banished from communicative language teaching — engage productive cognitive processes including contrastive analysis, metalinguistic reflection, and strategic competence. Kern (2014) similarly proposed that translation in the digital age constitutes a form of "transliteracy" — the ability to read, write, and interact across multiple media and language systems — that is increasingly essential for multilingual participation in global discourse.

The arrival of neural machine translation (NMT) systems of substantially improved quality — Google Translate's transformer-based engine, DeepL, and LLM-based translation — has accelerated this reconceptualization. When MT output was crude and unreliable, its pedagogical utility was limited. Now that MT produces largely accurate, natural-sounding translations for major language pairs, the pedagogical question shifts from "how do we prevent students from using MT?" to "how do we help students use MT as a scaffold for developing their own multilingual competence?"

### 13.4.2 MT as Comprehensible Input Generator

From an input perspective, MT can serve as a tool for making otherwise incomprehensible texts accessible — functioning as a scaffold toward Krashen's i+1. A learner of Japanese at an intermediate level might use MT to partially translate a newspaper article, reading the original Japanese text with MT-generated glosses for unfamiliar passages. This practice preserves engagement with authentic target language input while ensuring comprehension — arguably implementing Nation's (2001) extensive reading principle that learners should understand approximately 98% of running words for effective acquisition.

AI-enhanced MT systems can go further by providing not merely translations but graduated scaffolding. An intelligent MT tool might offer the learner a choice: full translation, key phrase translations only, first-language definitions of unfamiliar vocabulary in context, or syntactic parsing of complex sentences. This adaptive approach transforms MT from a binary comprehension/non-comprehension tool into a finely graduated scaffold that can be calibrated to the learner's developing competence. Several emerging platforms, including AI-powered parallel reading applications, are beginning to implement this graduated MT scaffolding model.

### 13.4.3 Post-Editing as a Learning Activity

One of the most promising pedagogical applications of MT leverages the imperfections of translation output. MT post-editing — the practice of reviewing and correcting MT output — engages learners in metalinguistic analysis that requires deep processing of both source and target language structures. Research by Lee (2020) and Niño (2020) has demonstrated that MT post-editing tasks engage learners in noticing (Schmidt, 1990) of grammatical, lexical, and pragmatic features that they might not attend to in conventional writing tasks.

The cognitive demands of post-editing align remarkably well with several SLA theoretical constructs. The task requires learners to notice discrepancies between the MT output and target language norms (Schmidt's Noticing Hypothesis), to generate alternative formulations (Swain's Output Hypothesis), and to reflect explicitly on linguistic form in context (metalinguistic awareness). When conducted collaboratively, post-editing additionally creates conditions for negotiation of meaning (Long's Interaction Hypothesis) as learners discuss and resolve translation problems together.

AI systems can enhance post-editing tasks by providing graduated support. An LLM might first generate a machine translation, then identify probable error types without correcting them (promoting noticing), then offer metalinguistic explanations upon request (supporting explicit learning), and finally provide a model revision for comparison (enabling hypothesis testing). This scaffolded post-editing workflow operationalizes multiple SLA learning mechanisms within a single task sequence.

### 13.4.4 The Risk of MT Dependency

Despite these affordances, legitimate concerns remain about MT's impact on multilingual development. Garcia and Pena (2011) cautioned that over-reliance on MT can reduce learners' motivation to develop productive competence in the target language, reasoning that if the machine can translate adequately, the human effort of acquiring the language may seem unnecessary. This concern echoes the broader paradox discussed in Chapter 6: AI tools that make language production easier may undermine the productive struggle that drives acquisition.

Empirical research on MT dependency remains limited but suggestive. Jolley and Maimone (2022) found that lower-proficiency learners were more likely to use MT as a substitute for genuine production rather than as a scaffold, while higher-proficiency learners tended to use MT more strategically — consulting translations to confirm hypotheses or to resolve specific difficulties. This finding suggests that the pedagogical value of MT depends significantly on learner proficiency and metacognitive awareness, and that AI systems incorporating MT should be designed with explicit guidance toward strategic rather than substitutive use.

---

## 13.5 Code-Switching and AI: Computational Challenges and Pedagogical Opportunities

### 13.5.1 The Computational Challenge of Code-Switched Input

Code-switching — the alternation between languages within a single discourse, sentence, or even word — presents formidable computational challenges for AI systems. Most NLP pipelines begin with a language identification step that assigns a single language label to the input text. Code-switched text defeats this initial classification, causing cascading failures in subsequent processing stages including tokenization, parsing, and generation.

Research in computational code-switching has expanded significantly since 2018 but remains in its early stages relative to monolingual NLP. Shared tasks at workshops such as the Computational Approaches to Linguistic Code-Switching (CALCS) series have established benchmarks for language identification in code-switched text, named entity recognition in code-switched data, and sentiment analysis of code-switched social media posts (Aguilar et al., 2020; Solorio et al., 2014). Performance on these tasks has improved substantially with transformer-based models but still lags significantly behind monolingual benchmarks.

For LLMs, code-switching capability varies dramatically by language pair and by the direction of the switch. GPT-4 and Claude handle English-Spanish code-switching with reasonable facility, likely because English-Spanish bilingual text is relatively common in their training data. However, these same models struggle with code-switching between languages less frequently represented in web text — Tagalog-English switching common in Filipino communication, for instance, or Hindi-English switching prevalent in Indian digital discourse. The implications for language learners are clear: AI systems will support code-switching practices for some language communities far more effectively than others, potentially widening existing digital linguistic divides.

### 13.5.2 Structural Constraints on Code-Switching and AI Processing

Linguistic research on code-switching has identified structural constraints governing where switches can and cannot occur. Poplack's (1980) free morpheme constraint and equivalence constraint, Myers-Scotton's (1993) Matrix Language Frame model, and more recent minimalist approaches (MacSwan, 2014) all propose that code-switching follows grammatical regularities rather than occurring randomly. These constraints are important for AI processing because they predict which code-switched utterances are structurally well-formed and which violate the grammatical systems of the relevant languages.

Current LLMs show mixed awareness of code-switching constraints. When prompted to generate code-switched text, they tend to produce utterances that respect surface-level patterns (switching at sentence or clause boundaries) but may violate more subtle structural constraints (switching within morphological boundaries or between tightly bound syntactic elements). This suggests that the models have learned distributional patterns of code-switching from their training data but have not acquired the underlying grammatical competence that governs code-switching in bilingual speakers — a finding consistent with the broader debate about whether LLMs possess genuine linguistic competence or merely sophisticated pattern matching (Bender & Koller, 2020).

### 13.5.3 AI Design for Code-Switching Contexts

Designing AI systems that appropriately handle code-switching requires moving beyond the "one language at a time" architecture that dominates current systems. Several approaches show promise. First, multilingual language models such as mBERT, XLM-R, and multilingual versions of major LLMs provide a foundation for processing mixed-language input by representing multiple languages in a shared embedding space (Conneau et al., 2020). These models can, in principle, process code-switched text without requiring language identification as a preprocessing step.

Second, deliberate inclusion of code-switched data in model training and fine-tuning can improve system performance on mixed-language input. Research by Winata et al. (2021) demonstrated that fine-tuning on synthetically generated code-switched data improved model performance on naturally occurring code-switching, even when the synthetic data imperfectly captured natural code-switching patterns. This finding suggests that AI developers can improve code-switching capability without requiring massive naturally occurring code-switched corpora — which are scarce for most language pairs.

Third, pedagogically oriented AI systems can be designed to actively engage with code-switching as a learning resource rather than treating it as noise to be filtered. An AI conversation partner for Spanish learners might be designed to model strategic code-switching — using English cognates when introducing new Spanish vocabulary, switching to English for metalinguistic explanations, and gradually reducing English support as the learner's proficiency develops. This approach aligns with translanguaging pedagogy (Garcia, Johnson, & Seltzer, 2017) while leveraging AI's ability to dynamically adjust its code-switching patterns to the individual learner's needs.

---

## 13.6 Heritage Language Learners and AI

### 13.6.1 The Heritage Learner Profile and AI Mismatch

Heritage language learners — individuals who grow up hearing and often speaking a language at home that differs from the dominant language of the broader society (Valdés, 2001) — present a particularly challenging case for AI language learning systems. Heritage speakers typically possess phonological and pragmatic competence that approaches or matches that of first-language speakers, combined with variable morphosyntactic and literacy skills that may be significantly below the level expected for their age or oral proficiency (Polinsky, 2018). This uneven profile does not map neatly onto the proficiency levels that AI systems use to calibrate content and feedback.

Consider the case of a heritage Spanish speaker in the United States who can engage in fluent conversation about family, food, and daily life but struggles with subjunctive morphology, formal register, and academic writing in Spanish. An AI system that assesses this learner's proficiency based on oral fluency might place them at an advanced level and provide texts and tasks that overwhelm their literacy skills. Conversely, a system that assesses based on a grammar test might place them at a beginning or intermediate level, delivering content insultingly below their communicative competence. Neither assessment captures the heritage learner's actual profile, which requires a more nuanced, multi-dimensional representation of linguistic competence.

### 13.6.2 Dialectal Variation and the Standard Language Ideology

Heritage language learners frequently speak dialectal or contact varieties of their heritage language that differ from the prestige standard variety. A heritage speaker of Mexican-American Spanish may use constructions such as "haiga" (subjunctive of haber), "asina" (thus), or "pos" (pues) — features stigmatized as "incorrect" in standard language ideology but representing systematic, rule-governed dialectal variation. Heritage Vietnamese speakers may use Southern Vietnamese phonological features that differ from the Northern standard typically taught in formal language classes.

Most AI language systems are trained on standard written varieties and reproduce standard language ideology in their corrections and assessments. An AI grammar checker will flag "haiga" as an error and suggest "haya," implicitly devaluing the learner's home variety. An AI pronunciation assessment will penalize Southern Vietnamese tonal patterns if calibrated to Northern standards. These corrections are not linguistically neutral; they carry social and political weight, potentially communicating to heritage learners that their home language practice is deficient — precisely the message that heritage language programs are designed to counteract (Leeman, 2015).

Designing AI systems for heritage learners requires dialect awareness and ideological sensitivity. At minimum, systems should be capable of distinguishing between dialectal features and genuine errors, providing information about register and context rather than blanket corrections. More ambitiously, AI systems could be designed to explicitly validate dialectal features while expanding learners' repertoires to include the standard variety — an additive approach consistent with the goals of heritage language pedagogy (Beaudrie, Ducar, & Potowski, 2014).

### 13.6.3 Family and Community Language Maintenance

AI tools offer potentially significant affordances for heritage language maintenance in families and communities. Heritage language loss is driven in large part by the reduced input and interaction opportunities available in the heritage language relative to the dominant societal language (Montrul, 2016). AI chatbots, story generators, and conversation partners could augment heritage language input in homes where parents' work schedules, mixed-language family dynamics, or community language shift limit the child's exposure to the heritage language.

Several emerging applications target this space. AI-powered bilingual storytime applications can generate personalized stories in the heritage language, providing rich input tailored to the child's interests and proficiency level. AI conversation partners can offer heritage language practice to adolescents who may be reluctant to speak the heritage language with family members but willing to engage with a non-judgmental AI interlocutor. AI-assisted homework help in the heritage language can extend the language's functional domains beyond the home, demonstrating to young heritage speakers that their language is useful for academic purposes and not merely a "kitchen language."

However, caution is warranted. AI-generated heritage language input may lack the cultural authenticity, emotional resonance, and pragmatic richness of genuine family and community interaction. A grandmother's stories carry cultural knowledge, identity messages, and relational warmth that no AI system can replicate. The risk is that families may view AI as a substitute for human heritage language interaction rather than a supplement to it — potentially accelerating rather than reversing language shift if AI replaces rather than augments human heritage language use (Fishman, 1991).

---

## 13.7 Low-Resource Languages and the Digital Divide

### 13.7.1 The Resource Hierarchy in NLP

Joshi et al.'s (2020) taxonomy of language resource availability reveals a stark digital divide. Category 0 ("the left-behinds") contains approximately 2,200 languages with essentially no digital NLP resources. Category 1 ("the scraping-bys") adds another 900 languages with minimal resources. Together, these categories represent roughly half of the world's living languages, spoken by hundreds of millions of people, for whom AI language technology is essentially nonexistent.

Even within the "resourced" categories, quality varies enormously. A learner of French can access AI tools — chatbots, grammar checkers, pronunciation coaches, adaptive reading systems — that perform at near-human levels. A learner of Wolof, spoken by approximately 10 million people in Senegal and the Gambia, will find AI tools that produce garbled text, fail to recognize spoken input, and provide grammatically incoherent feedback if they function at all. A learner of Mixtec, spoken by approximately 500,000 people in Mexico, will find no AI language learning tools whatsoever.

This resource hierarchy creates a perverse dynamic in which the languages that would benefit most from AI-assisted learning support — endangered and low-resource languages facing language shift, with limited teaching materials and few trained teachers — are precisely those for which AI tools are least available. The languages that least need AI support — major world languages with abundant materials, large teacher workforces, and extensive educational infrastructure — are those best served by current AI systems.

### 13.7.2 Low-Resource NLP and Language Revitalization

Despite these challenges, promising work is emerging at the intersection of low-resource NLP and language revitalization. Transfer learning techniques allow models trained on high-resource languages to be adapted for related low-resource languages with relatively small amounts of target language data (Zoph et al., 2016). Cross-lingual embeddings map words from different languages into a shared vector space, enabling zero-shot or few-shot learning for languages with minimal training data (Conneau et al., 2018).

Community-driven language documentation projects are beginning to leverage AI as a tool for accelerating the documentation and revitalization of endangered languages. The Endangered Languages Project (ELP), computational work on Yoloxochitl Mixtec (Yu et al., 2020), and ASR development for indigenous Australian languages (Foley et al., 2018) demonstrate how relatively small amounts of community-produced language data can be used to train useful (if imperfect) AI models that support language maintenance and revitalization efforts.

A particularly instructive case study involves AI-assisted documentation of Zapotec languages in Oaxaca, Mexico. Researchers working with Zapotec-speaking communities have used ASR and text processing tools, initially trained on higher-resource Mesoamerican languages and then fine-tuned on Zapotec data collected in collaboration with community members, to accelerate the transcription and analysis of oral histories and natural speech. The resulting tools are not comparable in quality to their English-language equivalents, but they are sufficient to meaningfully reduce the labor required for documentation — a critical contribution given the urgency of documenting languages with aging speaker populations.

### 13.7.3 Ethical Considerations in AI and Endangered Languages

The application of AI to endangered and low-resource languages raises significant ethical questions that the field has only begun to address. Data sovereignty — the right of indigenous and minority communities to control how their language data is collected, stored, used, and shared — is a fundamental concern. Community members who contribute language recordings and texts for documentation purposes may not have consented to their data being used to train commercial AI models, yet the boundaries between academic research, language documentation, and AI training data are increasingly porous (Holton, Leonard, & Pulsifer, 2022).

Cultural appropriateness is another concern. AI systems trained on language data may reproduce cultural knowledge — ceremonial language, kinship terms, traditional ecological knowledge — that communities consider sensitive or restricted. An AI chatbot that generates text in an indigenous language might produce culturally inappropriate combinations of words and concepts, or might make restricted knowledge accessible to outsiders in ways that violate community protocols.

Linguists and AI developers working with endangered language communities must adopt frameworks of reciprocity, consent, and community governance that go well beyond standard IRB protocols. The CARE principles for indigenous data governance (Carroll et al., 2020) — Collective Benefit, Authority to Control, Responsibility, and Ethics — provide a starting point, but implementation in the fast-moving AI landscape requires ongoing dialogue between technologists, linguists, and community stakeholders.

---

## 13.8 Designing AI for Multilingual Classrooms

### 13.8.1 The Multilingual Classroom Reality

Contemporary language classrooms are increasingly multilingual environments. A secondary ESL classroom in an American public school might include students whose home languages span Mandarin, Arabic, Somali, Spanish, and Dari. A university French class in London might include students who already speak Igbo, Polish, Urdu, and Cantonese in addition to English. Even in seemingly "homogeneous" settings, learners bring diverse linguistic resources — dialectal variation, familial languages learned partially in childhood, languages studied previously in school — that constitute their multilingual repertoires.

Effective pedagogy in multilingual classrooms recognizes and leverages this linguistic diversity as a resource for learning (Cenoz & Gorter, 2015; Cummins, 2007). Translanguaging pedagogy, as articulated by Garcia, Johnson, and Seltzer (2017), provides a framework for strategically deploying learners' full linguistic repertoires in service of both content learning and language development. In a translanguaging classroom, students might brainstorm in their home languages, discuss in mixed-language groups, write drafts incorporating multiple languages, and produce final texts in the target language — a process that values all languages in the room and leverages cross-linguistic connections for deeper learning.

### 13.8.2 Current AI Limitations in Multilingual Classrooms

Current AI language learning tools are poorly suited to multilingual classroom contexts. Most tools are designed for one-to-one interaction in a single language pair: a Spanish-speaking learner studying English, for example, or an English-speaking learner studying French. They do not accommodate the multilinguality of actual classrooms — the Somali-speaking learner in the ESL class who also speaks Arabic and is leveraging knowledge of Arabic script to learn English phonics, or the Polish-speaking learner in the French class whose knowledge of grammatical gender in Polish provides a bridge to French gender.

The tools' monolingual orientation also creates practical problems for classroom management. When every student in a multilingual classroom is using the same AI tutor configured for the same language pair, the AI cannot differentiate instruction based on learners' diverse L1 backgrounds. A feedback algorithm that works well for Spanish speakers learning English may be counterproductive for Mandarin speakers learning English, because the two groups face different phonological, morphosyntactic, and pragmatic challenges. True adaptive learning for multilingual classrooms requires adapting not just to the learner's proficiency level in the target language but to their entire multilingual profile.

### 13.8.3 Principles for Multilingual AI Design

Drawing on translanguaging theory, multi-competence research, and the practical realities of multilingual education, the following principles can guide the development of AI systems for multilingual language learning contexts:

**Principle 1: Support the full linguistic repertoire.** AI systems should be designed to receive, process, and respond to multilingual input without treating it as error. This means accepting code-switched utterances, providing responses that strategically incorporate the learner's known languages when pedagogically appropriate, and supporting the learner's ability to draw on cross-linguistic connections.

**Principle 2: Provide multilingual profiles, not monolingual levels.** Assessment and proficiency tracking should represent learners' capabilities across their linguistic repertoire — including receptive vs. productive skills, register variation, and domain-specific competencies — rather than assigning a single proficiency level in each named language. Heritage speakers, sequential multilinguals, and simultaneous bilinguals have qualitatively different profiles that monolingual proficiency scales cannot capture.

**Principle 3: Leverage cross-linguistic transfer.** AI systems should be aware of the typological relationships between a learner's known languages and the target language, and should actively leverage positive transfer while flagging areas of potential negative transfer. A Portuguese speaker learning Spanish should receive different instruction than a Japanese speaker learning Spanish, because the languages they bring to the task afford different types of cross-linguistic connection.

**Principle 4: Respect dialectal and contact varieties.** AI systems should distinguish between dialectal features and developmental errors, providing register-aware guidance rather than blanket corrections toward a single prestige standard. Learners should be informed about variation and register without being told that their home variety is "wrong."

**Principle 5: Design for classroom integration.** AI tools for multilingual classrooms should support collaborative as well as individual learning, allowing teachers to configure language resources for group activities, translanguaging tasks, and cross-linguistic analysis projects. The AI should be a tool that teachers can deploy flexibly, not a self-contained system that operates independently of classroom pedagogy.

**Principle 6: Prioritize underserved languages.** AI development for language learning should actively work to close the resource gap by investing in low-resource language capabilities, supporting community-driven language documentation, and ensuring that commercial AI language products do not exclusively serve high-resource languages.

---

## 13.9 Research on AI and Multilingual Development

### 13.9.1 Empirical Studies on AI and Multilingual Learners

Empirical research on AI systems' effectiveness with multilingual learners remains limited, but a growing body of work is beginning to illuminate key dynamics. Ziegler and Moeller (2024) investigated the performance of LLM-based chatbots for language practice across ten languages, finding statistically significant performance differentials that correlated with the language's representation in training data. English, Spanish, French, and Mandarin chatbot interactions received the highest quality ratings from human evaluators, while Arabic, Hindi, Swahili, and Vietnamese interactions showed notably more grammatical errors, pragmatic awkwardness, and cultural inaccuracies.

Kohnert and Ebert (2023) examined the impact of AI-generated corrective feedback on heritage Spanish speakers in the United States, finding that feedback calibrated to the standard variety without acknowledging dialectal features resulted in decreased motivation and increased negative attitudes toward the heritage language. When the AI was modified to include dialect-aware feedback that validated home variety features while introducing standard alternatives in context, learner engagement and motivation improved significantly. This study provides empirical support for the theoretical arguments advanced by heritage language educators and translanguaging scholars.

Research on MT as a pedagogical tool has expanded considerably. Briggs (2018) found that intermediate-level French learners who used MT as a planning tool for writing tasks produced more complex and more accurate French texts than control-group learners who did not use MT, while also demonstrating greater metalinguistic awareness in think-aloud protocols. Importantly, the MT-assisted group did not show reduced linguistic development over the semester-long study, countering concerns about MT-induced dependency.

### 13.9.2 Methodological Challenges in Multilingual AI Research

Research on AI and multilingual development faces distinctive methodological challenges. The heterogeneity of multilingual populations makes it difficult to form comparable experimental groups — heritage speakers, sequential bilinguals, simultaneous bilinguals, and receptive bilinguals in the "same" language differ so substantially in their linguistic profiles that treating them as a single group masks important variation. The dynamism of multilingual repertoires, which evolve constantly in response to changing social contexts, makes longitudinal measurement challenging.

Additionally, the researcher's own linguistic ideology can influence study design and interpretation. A study that defines "improvement" as increased conformity to monolingual native-speaker norms operationalizes a very different construct than one that defines "improvement" as expanded multilingual repertoire, increased translanguaging fluency, or enhanced metalinguistic awareness. These definitional choices are not neutral; they reflect (and reproduce) particular ideologies of language and multilingualism.

Future research on AI and multilingual development should adopt designs that (a) represent the diversity of multilingual profiles within study populations, (b) measure multilingual competence through multiple dimensions rather than monolingual proficiency scales, (c) attend to the social and identity dimensions of AI-mediated multilingual practice, and (d) involve multilingual community members as research partners rather than merely as research subjects.

### 13.9.3 Emerging Research Directions

Several promising research directions are emerging at the intersection of AI and multilingual development. First, studies of AI-mediated translanguaging in educational settings are beginning to document how learners use AI tools to navigate between languages in ways that support both content learning and language development (Lin & He, 2024). These studies employ discourse analysis and ethnographic methods to capture the fine-grained interactional dynamics of translanguaging with AI.

Second, computational research on cross-lingual transfer in multilingual language models is generating insights relevant to SLA theory. Studies demonstrating that multilingual models represent syntactic structures shared across languages in similar embedding space regions (Chi, Hewitt, & Manning, 2020) provide computational evidence for the "common underlying proficiency" hypothesized by Cummins (1979) — the idea that multilingual speakers possess a shared cognitive foundation that underlies surface-level language-specific competence.

Third, design-based research (DBR) projects are developing and testing AI prototypes specifically designed for multilingual contexts. These projects, which iterate between design, implementation, evaluation, and redesign, are producing both practical AI tools and theoretical insights about what multilingual learners need from AI systems (Vogel & Garcia, 2023). The DBR approach is particularly well-suited to this domain because the novelty of AI-multilingual interaction means that researchers cannot simply apply existing design principles but must develop new ones through iterative engagement with multilingual learners and communities.

---

## 13.10 Toward a Multilingual AI Future

### 13.10.1 The Promise of Multilingual Foundation Models

Recent developments in multilingual AI offer cautious grounds for optimism. Multilingual foundation models — large models trained intentionally on balanced multilingual data — are beginning to narrow the performance gap between high-resource and lower-resource languages. Models such as BLOOM, which was trained with explicit attention to African and South Asian language representation, and SEA-LION, focused on Southeast Asian languages, demonstrate that targeted data curation can meaningfully improve AI performance for underserved languages.

The rise of open-source multilingual models also creates opportunities for community-driven development. Unlike proprietary systems controlled by Silicon Valley corporations with little incentive to invest in Quechua or Yoruba capability, open-source models can be fine-tuned by researchers and community members who possess both the linguistic expertise and the cultural knowledge necessary to develop appropriate AI tools for specific language communities.

### 13.10.2 Integrating Multilingual AI into SLA Theory

The intersection of AI and multilingualism also presents opportunities for theoretical advancement in SLA. As AI systems become more capable of processing and generating multilingual text, they provide new tools for testing theoretical claims about the nature of multilingual competence. If an AI model trained on balanced multilingual data demonstrates cross-linguistic facilitation in language production — producing more fluent output in Language A after fine-tuning on Language B — this would provide computational evidence relevant to theories of cross-linguistic transfer and multi-competence.

Conversely, the failures of AI systems in multilingual contexts can illuminate aspects of human multilingual competence that current computational approaches fail to capture. If AI systems consistently struggle with the pragmatic dimensions of code-switching — knowing when a switch is socially appropriate, emotionally charged, or identity-relevant — this difficulty highlights the social embeddedness of multilingual practice that purely computational models cannot replicate.

### 13.10.3 Summary and Implications

The relationship between AI and multilingualism is characterized by a fundamental tension: the most powerful language technologies in human history have been built on assumptions about language that the field of applied linguistics has spent decades dismantling. The monolingual bias in AI — from training data through tokenization, evaluation, and deployment — is not merely a technical limitation to be engineered away but an ideological orientation that must be recognized and actively countered.

For language learners, the consequences of this bias are real and immediate. Heritage speakers receive feedback that devalues their home varieties. Multilingual learners are forced into monolingual interaction modes that suppress their natural communicative practices. Speakers of low-resource languages are excluded from the affordances of AI-assisted learning entirely. These are not future problems to be anticipated but present realities to be addressed.

The path forward requires collaboration between AI developers, applied linguists, and multilingual communities. It requires investment in multilingual training data, multilingual evaluation benchmarks, and multilingual design principles. It requires centering the needs and knowledge of multilingual users — who constitute the global majority — rather than treating them as edge cases in systems designed for monolingual English speakers. And it requires the theoretical courage to design AI systems that reflect what we know about the nature of multilingual competence rather than what is technically convenient.

The multilingual future of AI in language learning is not a given; it is a choice. The theories and evidence reviewed in this chapter provide a clear direction. Whether the field has the will to follow that direction remains an open question — one that will shape the language learning experiences of millions of multilingual learners for decades to come.

---

## Discussion Questions

1. How does Cook's multi-competence framework challenge the design assumptions of current AI language learning platforms? What specific design changes would be required to align AI tools with a multi-competence view of multilingualism?

2. Consider a heritage language learner you know or have taught. How would current AI language tools serve this learner? What features would need to be added, modified, or removed to appropriately support heritage language development?

3. Garcia and Wei argue that translanguaging is not a deficiency but a competence. How might an AI language tutor be designed to support translanguaging practices while still developing learners' competence in specific named languages for academic or professional purposes?

4. Examine a commercial AI language learning tool (e.g., Duolingo, Babbel, ChatGPT, Speak). Analyze its handling of multilingual input. Does it accept code-switching? How does it respond to dialectal variation? What monolingual assumptions are embedded in its design?

5. Discuss the ethical considerations involved in using AI to document and revitalize endangered languages. How can the CARE principles (Collective Benefit, Authority to Control, Responsibility, Ethics) be operationalized in AI-language revitalization projects?

---

## Practical Applications: Try This Monday

**Activity 1: Multilingual Repertoire Mapping**
Have students create a visual map of their linguistic repertoire — all languages, dialects, registers, and specialized vocabularies they use. Then ask them to interact with an AI chatbot using their natural multilingual communication style (including code-switching). Document how the AI responds. Discuss what the AI's responses reveal about its assumptions about language.

**Activity 2: MT Post-Editing Workshop**
Generate a machine translation of a short authentic text (news article, song lyrics, or social media post) in the target language. Have students work in pairs to identify and correct errors, categorizing them (grammatical, lexical, pragmatic, cultural). Compare the post-edited versions to discuss how different multilingual perspectives led to different revision decisions.

**Activity 3: Dialect-Aware AI Interaction**
If teaching a language with significant dialectal variation (Spanish, Arabic, Chinese), have students input dialectal features into an AI grammar checker or chatbot. Document which features are flagged as errors. Research whether the flagged features are genuine errors or dialectal variants. Create a class "dialect awareness guide" documenting the AI's biases.

---

## References

Aguilar, G., Kar, S., & Solorio, T. (2020). LinCE: A centralized benchmark for linguistic code-switching evaluation. *Proceedings of LREC 2020*, 1803-1813.

Beaudrie, S. M., Ducar, C., & Potowski, K. (2014). *Heritage language teaching: Research and practice*. McGraw-Hill.

Bender, E. M., & Koller, A. (2020). Climbing towards NLU: On meaning, form, and understanding in the age of data. *Proceedings of the 58th Annual Meeting of the ACL*, 5185-5198.

Briggs, N. (2018). Neural machine translation tools in the language learning classroom: Students' use, perceptions, and analyses. *JALT CALL Journal*, 14(1), 3-24.

Canagarajah, S. (2013). *Translingual practice: Global Englishes and cosmopolitan relations*. Routledge.

Carroll, S. R., Garba, I., Figueroa-Rodriguez, O. L., Holbrook, J., Lovett, R., Materechera, S., ... & Hudson, M. (2020). The CARE principles for indigenous data governance. *Data Science Journal*, 19(1), 43.

Cenoz, J., & Gorter, D. (2015). Multilingual education: Between language learning and translanguaging. *Cambridge University Press*.

Chi, E. A., Hewitt, J., & Manning, C. D. (2020). Finding universal grammatical relations in multilingual BERT. *Proceedings of the 58th Annual Meeting of the ACL*, 5564-5577.

Conneau, A., Khandelwal, K., Goyal, N., Chaudhary, V., Wenzek, G., Guzman, F., ... & Stoyanov, V. (2020). Unsupervised cross-lingual representation learning at scale. *Proceedings of the 58th Annual Meeting of the ACL*, 8440-8451.

Conneau, A., Lample, G., Ranzato, M., Denoyer, L., & Jégou, H. (2018). Word translation without parallel data. *Proceedings of ICLR 2018*.

Cook, V. (1991). The poverty-of-the-stimulus argument and multicompetence. *Second Language Research*, 7(2), 103-117.

Cook, V. (2001). Using the first language in the classroom. *Canadian Modern Language Review*, 57(3), 402-423.

Cook, V. (2016). Premises of multi-competence. In V. Cook & L. Wei (Eds.), *The Cambridge handbook of linguistic multi-competence* (pp. 1-25). Cambridge University Press.

Cummins, J. (1979). Linguistic interdependence and the educational development of bilingual children. *Review of Educational Research*, 49(2), 222-251.

Cummins, J. (2007). Rethinking monolingual instructional strategies in multilingual classrooms. *Canadian Journal of Applied Linguistics*, 10(2), 221-240.

Dodge, J., Sap, M., Marasovic, A., Agnew, W., Ilharco, G., Groeneveld, D., & Smith, N. A. (2021). Documenting large webtext corpora: A case study on the Colossal Clean Crawled Corpus. *Proceedings of EMNLP 2021*, 1286-1305.

Fishman, J. A. (1991). *Reversing language shift: Theoretical and empirical foundations of assistance to threatened languages*. Multilingual Matters.

Foley, B., Arnold, J., Coto-Solano, R., Durantin, G., Ellison, T. M., van Esch, D., ... & Wiles, J. (2018). Building speech recognition systems for language documentation. *Proceedings of the 3rd Workshop on the Use of Computational Methods in the Study of Endangered Languages*, 94-104.

Garcia, O., Johnson, S. I., & Seltzer, K. (2017). *The translanguaging classroom: Leveraging student bilingualism for learning*. Caslon Publishing.

Garcia, O., & Pena, C. M. (2011). Transformative translanguaging strategies. In C. Celic & K. Seltzer (Eds.), *Translanguaging: A CUNY-NYSIEB guide for educators*. CUNY-NYSIEB.

Garcia, O., & Wei, L. (2014). *Translanguaging: Language, bilingualism, and education*. Palgrave Macmillan.

Gonzalez-Davies, M. (2004). *Multiple voices in the translation classroom*. John Benjamins.

Gonzalez-Davies, M. (2014). Towards a plurilingual development paradigm: From spontaneous to informed use of translation in additional language learning. *The Interpreter and Translator Trainer*, 8(1), 8-31.

Grosjean, F. (2010). *Bilingual: Life and reality*. Harvard University Press.

Holton, G., Leonard, W. Y., & Pulsifer, P. L. (2022). Indigenous peoples, ethics, and linguistic data. In A. Berez-Kroeker et al. (Eds.), *The Open Handbook of Linguistic Data Management* (pp. 49-60). MIT Press.

Jolley, J. R., & Maimone, L. (2022). Thirty years of machine translation in language teaching and learning: A review of the literature. *L2 Journal*, 14(1), 1-25.

Joshi, P., Santy, S., Buber, A., Bali, K., & Choudhury, M. (2020). The state and fate of linguistic diversity and inclusion in the NLP world. *Proceedings of the 58th Annual Meeting of the ACL*, 6282-6293.

Kern, R. (2014). Technology as Pharmakon: The promise and perils of the internet for foreign language education. *Modern Language Journal*, 98(1), 340-357.

Kohnert, K., & Ebert, K. D. (2023). AI-generated feedback for heritage language learners: Effects of dialect-aware vs. standard-only feedback on motivation and engagement. *Language Learning & Technology*, 27(2), 1-24.

Lee, S. M. (2020). The impact of using machine translation on EFL students' writing. *Computer Assisted Language Learning*, 33(3), 157-175.

Leeman, J. (2015). Heritage language education and identity in the United States. *Annual Review of Applied Linguistics*, 35, 100-119.

Lin, A. M. Y., & He, P. (2024). Translanguaging with AI: Multimodal practices in multilingual classrooms. *Applied Linguistics*, 45(1), 88-107.

MacSwan, J. (2014). Programs and proposals in codeswitching research: Unconstraining theories of bilingual language mixing. In J. MacSwan (Ed.), *Grammatical theory and bilingual codeswitching* (pp. 1-33). MIT Press.

Makoni, S., & Pennycook, A. (2007). *Disinventing and reconstituting languages*. Multilingual Matters.

Montrul, S. (2016). *The acquisition of heritage languages*. Cambridge University Press.

Myers-Scotton, C. (1993). *Duelling languages: Grammatical structure in codeswitching*. Clarendon Press.

Nation, I. S. P. (2001). *Learning vocabulary in another language*. Cambridge University Press.

Niño, A. (2020). Exploring the use of online machine translation for independent language learning. *Research in Learning Technology*, 28, 2402.

Ortega, L. (2014). Ways forward for a bi/multilingual turn in SLA. In S. May (Ed.), *The multilingual turn: Implications for SLA, TESOL, and bilingual education* (pp. 32-53). Routledge.

Otheguy, R., Garcia, O., & Reid, W. (2015). Clarifying translanguaging and deconstructing named languages: A perspective from linguistics. *Applied Linguistics Review*, 6(3), 281-307.

Polinsky, M. (2018). *Heritage languages and their speakers*. Cambridge University Press.

Poplack, S. (1980). Sometimes I'll start a sentence in Spanish y termino en español: Toward a typology of code-switching. *Linguistics*, 18(7-8), 581-618.

Ruder, S., Vulić, I., & Søgaard, A. (2021). A survey of cross-lingual word embedding models. *Journal of Artificial Intelligence Research*, 65, 569-631.

Schmidt, R. (1990). The role of consciousness in second language learning. *Applied Linguistics*, 11(2), 129-158.

Sennrich, R., Haddow, B., & Birch, A. (2016). Neural machine translation of rare words with subword units. *Proceedings of the 54th Annual Meeting of the ACL*, 1715-1725.

Solorio, T., Blair, E., Maharjan, S., Bethard, S., Diab, M., Ghoneim, M., ... & Fung, P. (2014). Overview for the first shared task on language identification in code-switched data. *Proceedings of the First Workshop on Computational Approaches to Code Switching*, 62-72.

Valdés, G. (2001). Heritage language students: Profiles and possibilities. In J. K. Peyton, D. A. Ranard, & S. McGinnis (Eds.), *Heritage languages in America: Preserving a national resource* (pp. 37-80). Center for Applied Linguistics.

Vogel, S., & Garcia, O. (2023). Designing AI for multilingual classrooms: A design-based research approach. *Language Teaching Research*, 27(4), 891-912.

Wei, L. (2008). Research perspectives on bilingualism and multilingualism. In L. Wei & M. Moyer (Eds.), *The Blackwell handbook of research methods on bilingualism and multilingualism* (pp. 3-17). Blackwell.

Winata, G. I., Madotto, A., Lin, Z., Liu, R., Yosinski, J., & Fung, P. (2021). Language models are few-shot multilingual learners. *Proceedings of the 1st Workshop on Multilingual Representation Learning*, 1-15.

Yu, K. M., Lee, H., & Piantadosi, S. T. (2020). Computational approaches to endangered language documentation. *Annual Review of Linguistics*, 6, 347-370.

Ziegler, N., & Moeller, A. J. (2024). LLM chatbot performance across languages: Implications for equitable AI-assisted language learning. *Computer Assisted Language Learning*, 37(1), 45-68.

Zoph, B., Yuret, D., May, J., & Knight, K. (2016). Transfer learning for low-resource neural machine translation. *Proceedings of EMNLP 2016*, 1568-1575.
