# Chapter 7: Feedback, Error Correction, and AI

## The Tireless Interlocutor

---

## 7.1 Introduction: The Promise and Peril of Unlimited Feedback

Few constructs in second language acquisition (SLA) research have generated as much empirical attention -- and as much pedagogical controversy -- as corrective feedback (CF). From Krashen's (1982) provocative claim that error correction is essentially useless for acquisition, through the interactionist turn that positioned feedback as a catalyst for noticing and restructuring (Long, 1996; Schmidt, 1990), to the meta-analytic syntheses that have largely settled the question of whether CF "works" while opening new questions about how, when, and for whom (Li, 2010; Lyster & Saito, 2010; Mackey & Goo, 2007), the corrective feedback literature represents one of the most robust empirical traditions in the field. It is also, not coincidentally, the domain where artificial intelligence has made its most visible incursion into language education.

The reason is straightforward: feedback is expensive. In a classroom of twenty-five learners, each producing oral and written output across multiple linguistic domains, the human teacher faces an impossible triage. Which errors to address? When? How explicitly? The research literature offers guidance -- recasts for oral interaction, metalinguistic clues for certain grammatical targets, written corrective feedback calibrated to developmental readiness -- but the practical reality is that most learners receive far less feedback than the research would recommend. A teacher who provides individual written feedback on every student essay, addressing lexical, syntactic, morphological, and discourse-level errors with appropriate metalinguistic commentary, is a teacher who has no time left for anything else.

Artificial intelligence appears to resolve this constraint entirely. Automated writing evaluation (AWE) systems such as Grammarly, Cambridge Write & Improve, and ETS's Criterion can process thousands of texts simultaneously, providing immediate feedback on grammar, mechanics, vocabulary, and even discourse organization. Large language models (LLMs) such as ChatGPT, Claude, and Gemini can generate detailed metalinguistic explanations, provide recasts, elicit self-correction, and sustain extended corrective dialogues that would exhaust a human tutor. Speech recognition systems can flag pronunciation errors in real time. The AI interlocutor never tires, never loses patience, and never runs out of time.

Yet the SLA literature has spent four decades demonstrating that corrective feedback is not a monolithic intervention whose effectiveness scales linearly with quantity. The type of feedback matters (Lyster & Ranta, 1997). The timing matters (Doughty, 2001). The target structure matters (Ammar & Spada, 2006). The learner's developmental readiness matters (Mackey & Philp, 1998). The social and affective context matters (Aljaafreh & Lantolf, 1994). The question, therefore, is not whether AI can provide more feedback -- it self-evidently can -- but whether the feedback AI provides is the right kind, delivered at the right moment, targeting the right structures, for the right learners, in the right way.

This chapter examines that question through a systematic analysis of AI-generated corrective feedback against the theoretical frameworks and empirical findings that have shaped the CF literature in SLA. It begins with a review of the corrective feedback taxonomy that has organized research for nearly three decades, then evaluates how AI systems map onto that taxonomy, examines the critical role of learner noticing and uptake, assesses automated writing evaluation systems against the written CF literature, and concludes with a principled framework for determining when AI feedback helps and when it hinders acquisition.

---

## 7.2 Corrective Feedback in SLA: Theoretical Foundations

### 7.2.1 The Interactionist Case for Feedback

The theoretical rationale for corrective feedback in SLA rests on several converging frameworks, each emphasizing a different mechanism through which feedback facilitates acquisition. Long's (1996) updated Interaction Hypothesis positioned negotiation of meaning -- and the corrective feedback embedded within it -- as a primary mechanism connecting input, internal learner capacities, and output. When communication breaks down and interlocutors negotiate to resolve the breakdown, learners receive evidence about the gap between their interlanguage and target language norms. This negative evidence, Long argued, is particularly valuable because it arrives precisely when the learner is attending to meaning, creating optimal conditions for the cognitive processing that drives acquisition.

Schmidt's (1990, 2001) Noticing Hypothesis provided the cognitive mechanism: for input to become intake, learners must consciously notice features of the input, including the gap between their own production and target forms. Corrective feedback, by drawing attention to errors, serves as a noticing trigger. The effectiveness of different feedback types, from this perspective, depends on their capacity to make the relevant form-meaning connection salient enough for the learner to notice it amidst the complex, multi-dimensional processing demands of real-time communication.

Swain's (1985, 1995) Output Hypothesis added another dimension: the act of producing output and receiving feedback on that output enables learners to test hypotheses about the target language, notice gaps in their own knowledge, and engage in metalinguistic reflection. Feedback is not merely corrective information; it is a catalyst for the kind of deeper processing that transforms declarative knowledge into proceduralized competence.

From a sociocultural perspective, Aljaafreh and Lantolf (1994) reframed corrective feedback as mediation within the learner's zone of proximal development (ZPD). Effective feedback, on this view, is not a fixed intervention applied uniformly but a graduated, negotiated process in which the more knowledgeable interlocutor provides the minimum assistance necessary for the learner to self-correct. The regulatory scale they proposed -- moving from implicit to increasingly explicit feedback -- has profound implications for AI systems, which must determine not just what feedback to provide but how much scaffolding the individual learner requires.

### 7.2.2 Lyster and Ranta's Corrective Feedback Taxonomy

The framework that has most durably organized CF research is Lyster and Ranta's (1997) taxonomy, developed from their observational study of corrective feedback in French immersion classrooms. Their classification identified six feedback types, which subsequent research has grouped into two broad categories:

**Reformulations** (input-providing):

1. **Recasts**: The teacher reformulates all or part of the learner's erroneous utterance without explicitly indicating an error has occurred. Example: Learner: "Yesterday I go to the store." Teacher: "Oh, you went to the store?" Recasts are the most frequent feedback type in naturalistic classroom interaction (Lyster & Ranta, 1997; Sheen, 2006) and in conversational contexts generally. They maintain communicative flow while providing positive evidence of the target form.

2. **Explicit correction**: The teacher clearly indicates the error and provides the correct form. Example: "No, we don't say 'goed.' The past tense of 'go' is 'went.'" This is the most transparent feedback type, leaving no ambiguity about the error or its correction.

**Prompts** (output-pushing):

3. **Clarification requests**: The teacher indicates that the utterance was not understood, prompting the learner to reformulate. Example: "Sorry, what did you say?" or "I don't understand." This signals a communication breakdown without identifying the specific error.

4. **Metalinguistic clues**: The teacher provides comments, information, or questions related to the well-formedness of the learner's utterance without providing the correct form. Example: "Can you think about the tense you need here?" or "Remember, in English we use the past tense for completed actions."

5. **Elicitation**: The teacher directly elicits a reformulation from the learner through various techniques -- strategic pauses, questions, or requests for reformulation. Example: "Yesterday you...?" (with rising intonation, prompting the learner to complete the utterance correctly).

6. **Repetition**: The teacher repeats the learner's erroneous utterance, typically with rising intonation or emphatic stress on the error, signaling that something is wrong. Example: "You *goed* to the store?" (with emphasis on "goed").

The critical distinction between these categories, which has driven much subsequent research, is that reformulations provide the correct form while prompts withhold it, requiring the learner to retrieve or reconstruct the target form from their own developing system. This distinction maps onto a fundamental question in SLA: Is it more beneficial for learners to receive correct models (input-based learning) or to be pushed to produce modified output (output-based learning)?

### 7.2.3 Meta-Analytic Evidence on Feedback Effectiveness

Three decades of research following Lyster and Ranta's taxonomy have produced a substantial empirical base, synthesized in several important meta-analyses. Li's (2010) comprehensive meta-analysis of 33 studies found an overall positive effect for corrective feedback on L2 development (d = 0.61 on immediate posttests, d = 0.53 on delayed posttests), with important moderating variables. Explicit feedback types showed larger effects than implicit types in the short term, though the advantage narrowed on delayed measures. Lyster and Saito's (2010) meta-analysis of 15 classroom-based studies confirmed that prompts generated larger effect sizes than recasts, particularly for morphosyntactic targets.

However, the picture is more nuanced than these general trends suggest. Mackey and Goo (2007) found that recasts were effective for short-term gains while prompts showed stronger durability effects. Sheen's (2011) research demonstrated that the effectiveness of recasts varies dramatically based on contextual factors: recasts delivered in communicatively oriented classroom discourse are often ambiguous and go unnoticed, while recasts in more form-focused contexts are more salient and more effective. The learner's developmental readiness also mediates effectiveness: Mackey and Philp (1998) found that intensive recasts were particularly beneficial for learners who were developmentally ready to acquire the target structure.

For written corrective feedback (WCF), the research trajectory has been equally complex. Truscott (1996) famously argued that grammar correction is not only ineffective but harmful, a claim that generated extensive debate. Ferris (1999) countered that the evidence was insufficient to support such a sweeping conclusion. Subsequent research, including Bitchener and Knoch's (2010) longitudinal studies and Shintani and Ellis's (2013) work on metalinguistic explanation, has largely demonstrated that focused written CF (targeting specific error types) is effective for improving accuracy on treated structures, while unfocused CF (targeting all errors simultaneously) shows weaker or inconsistent effects.

This body of research establishes several principles that must inform any evaluation of AI-generated feedback: (a) feedback type interacts with target structure, learner proficiency, and context; (b) the distinction between input-providing and output-pushing feedback has pedagogical significance; (c) focused feedback outperforms unfocused feedback for accuracy development; (d) developmental readiness modulates feedback effectiveness; and (e) the social and interactional context of feedback delivery affects its uptake and utility.

---

## 7.3 How AI Provides Corrective Feedback: A Taxonomy Analysis

### 7.3.1 Mapping AI Feedback onto Lyster and Ranta's Categories

To evaluate AI corrective feedback rigorously, we must first determine which types of feedback from Lyster and Ranta's taxonomy AI systems can deliver and with what fidelity. The mapping reveals both capabilities and fundamental limitations.

**Explicit correction**: This is the feedback type most naturally suited to AI systems and the one they deliver most frequently and reliably. Grammar checkers (Grammarly, LanguageTool, ProWritingAid), AWE systems (Criterion, Write & Improve, Pigai), and LLMs can all identify errors and provide correct forms with explanations. When Grammarly underlines "Yesterday I go to the store" and offers "went" with the explanation "Use past simple for completed actions," it is delivering textbook explicit correction. AI systems excel here because explicit correction requires pattern recognition (identifying the error), knowledge retrieval (accessing the correct form), and explanation generation (articulating the rule) -- all tasks well within current computational capabilities.

**Recasts**: LLM-based conversational agents can deliver recasts with reasonable fidelity. When a learner writes "I am agree with you" and the AI responds "I agree -- the economic situation is certainly concerning," the AI has reformulated the erroneous form within a meaningful communicative response. However, the quality of AI recasts differs from human recasts in important ways. Human recasts in natural conversation are embedded in genuine communicative intent; the teacher is simultaneously reformulating and responding to the content of the learner's message. AI recasts, while structurally similar, lack the communicative authenticity that makes human recasts pragmatically natural. The AI is performing a recast because it has been instructed (or has learned) to correct errors, not because it needs to confirm its understanding for communicative purposes.

**Metalinguistic clues**: LLMs can generate sophisticated metalinguistic commentary, often exceeding what classroom teachers provide in terms of detail and accuracy. An LLM can explain the difference between the present perfect and simple past in English, cite the relevant rule, provide multiple examples, and relate the structure to the learner's L1 if known. However, the timing and contextualization of metalinguistic feedback in AI systems differs fundamentally from classroom interaction, where a teacher's metalinguistic clue emerges from reading the learner's specific utterance in a specific communicative context and calibrating the hint to what the teacher knows about the learner's developmental level.

**Clarification requests**: AI conversational agents can simulate clarification requests ("I'm not sure what you mean -- could you rephrase that?"), but there is a fundamental authenticity problem. A human clarification request is genuine: the interlocutor did not understand. An AI clarification request is performative: the system likely did "understand" the erroneous utterance perfectly well (LLMs are trained on vast amounts of non-standard language) and is pretending not to understand as a pedagogical strategy. Whether this pedagogical simulation carries the same acquisitional weight as genuine negotiation for meaning is an open empirical question, but the theoretical implications are significant. Long's (1996) Interaction Hypothesis positioned negotiation of meaning as facilitative precisely because the communicative need to be understood motivates the learner's cognitive investment in restructuring. When the "need" is artificial, the motivational mechanism may be weakened.

**Elicitation and repetition**: These feedback types are the most challenging for AI systems because they require real-time, contextually sensitive withholding of information combined with pragmatically appropriate prompting. An AI can be programmed to repeat a learner's error with emphasis ("You said 'I goed to the store'?") or to use strategic pauses and partial completions ("Yesterday you...?"). Some purpose-built language tutoring systems do implement these strategies. But the interactional subtlety required -- reading the learner's facial expression, sensing hesitation, adjusting the level of explicitness based on the learner's apparent confusion or confidence -- remains beyond current AI capabilities in text-based interaction and only partially available in multimodal systems.

### 7.3.2 The Explicitness Continuum in AI Feedback

One of the most significant findings in the CF literature is that the optimal level of explicitness is not fixed but varies by learner, target structure, and context. Aljaafreh and Lantolf's (1994) regulatory scale, grounded in Vygotskian sociocultural theory, proposed that effective feedback begins at the most implicit level and becomes progressively more explicit only as needed. The ideal is the minimum assistance necessary for the learner to self-correct, because self-correction represents internalization of the regulatory mechanism -- the learner moving from other-regulation (needing external help) to self-regulation (managing their own linguistic performance).

Current AI systems overwhelmingly default to the explicit end of the continuum. Grammarly identifies the error, provides the correction, and explains the rule -- all in a single feedback event. This is maximally explicit and maximally efficient from an information-delivery standpoint, but it is also maximally disempowering from a sociocultural perspective. The learner is given no opportunity to notice the error independently, no opportunity to attempt self-correction, and no graduated scaffolding that respects their ZPD.

LLM-based tutoring systems have more flexibility. A well-designed prompt can instruct the LLM to first hint at an error, then provide a metalinguistic clue if the learner cannot identify it, then offer the correction only as a last resort. Several educational AI platforms (e.g., Khan Academy's Khanmigo, Duolingo's LLM-powered features) have implemented versions of this graduated approach. However, the effectiveness of such systems depends entirely on the quality of the prompt engineering or system design, and there is currently no mechanism for the AI to dynamically assess the learner's ZPD in real time the way a skilled human tutor does -- reading hesitation, partial attempts, and affective states to calibrate the next move.

### 7.3.3 Feedback on What? Error Types and AI Capabilities

AI systems do not correct all error types with equal competence, and this differential capability has implications for acquisition that go beyond mere accuracy of error detection.

**Morphosyntactic errors** represent the strongest domain for AI feedback. Subject-verb agreement, tense formation, article usage, preposition selection, and other rule-governed or statistically predictable patterns are precisely the kind of regularities that both traditional grammar checkers and LLMs handle well. This is fortunate in one sense -- morphosyntactic accuracy is a major focus of the CF literature (Lyster, 2004; Sheen, 2007) -- but problematic in another, because it may create a feedback ecology in which learners receive abundant correction on precisely those features that are most amenable to explicit, rule-based learning while receiving little feedback on the aspects of language use that require more nuanced, context-dependent judgment.

**Lexical errors** -- inappropriate word choice, collocation violations, register mismatches -- are handled with moderate competence by LLMs, which have strong statistical representations of word co-occurrence patterns. However, AI feedback on lexical errors tends toward substitution ("Consider using 'obtain' instead of 'get' in formal writing") rather than the kind of extended lexical negotiation that promotes deep vocabulary processing (Laufer & Hulstijn, 2001).

**Pragmatic errors** -- inappropriate speech acts, politeness violations, register failures, culturally inappropriate communication strategies -- represent the weakest domain for AI feedback. While LLMs can identify gross pragmatic violations ("This email is too informal for a job application"), the subtle, context-dependent nature of pragmatic competence means that AI feedback in this domain is often generic, culturally biased toward Anglo-American norms, and insufficiently sensitive to the specific communicative context.

**Discourse-level errors** -- problems with coherence, cohesion, rhetorical organization, and argumentation structure -- occupy a middle ground. AWE systems like Criterion and Write & Improve include discourse-level feedback features, and LLMs can provide commentary on essay organization and logical flow. However, the quality of such feedback varies considerably, and research suggests that learners find AI discourse feedback less actionable than sentence-level corrections (Stevenson & Phakiti, 2014).

---

## 7.4 Automated Writing Evaluation Systems: The Leading Edge of AI Feedback

### 7.4.1 The AWE Landscape

Automated writing evaluation represents the most mature application of AI corrective feedback in language education, with a research base extending back to Page's (1966) Project Essay Grade. Contemporary AWE systems fall into two broad categories: formative systems designed to provide feedback during the writing process, and summative systems designed to score completed texts.

**ETS Criterion** uses the e-rater engine, a hybrid of statistical NLP and rule-based grammar checking, to provide feedback on grammar, usage, mechanics, style, and discourse structure. Developed for both L1 and L2 writers, Criterion represents two decades of iterative development and has been the subject of extensive validity research (Attali & Burstein, 2006; Weigle, 2010).

**Cambridge Write & Improve** is a free tool developed by Cambridge University Press & Assessment specifically for English language learners. It uses machine learning models trained on the Cambridge Learner Corpus to provide CEFR-level scores and targeted feedback. Its pedagogical design encourages iterative revision, aligning with process-writing approaches (Ballance, 2019).

**Grammarly**, while not designed specifically for L2 learners, has become one of the most widely used writing feedback tools among English learners worldwide. Its real-time, inline feedback model differs from traditional AWE submission-and-review cycles, providing corrections as the learner types. The Premium version offers style, tone, and clarity suggestions beyond basic grammar checking.

**Chinese AWE systems**, including Pigai (used by over 100 million Chinese English learners) and iWrite, represent a massive but often overlooked segment of the AI feedback landscape. Pigai's integration into Chinese university English programs has created what may be the largest-scale deployment of AI corrective feedback in language education history, generating a rich body of Chinese-language research that deserves greater attention in Western applied linguistics (Zhang, 2020).

### 7.4.2 What AWE Systems Correct Well

Research on AWE effectiveness has consistently identified specific domains where automated feedback contributes to measurable improvement. Dikli and Bleyle (2014) found that ETS Criterion feedback led to significant improvement in grammatical accuracy across multiple drafts, particularly for article errors, subject-verb agreement, and verb tense. Kellogg, Whiteford, and Quinlan (2010) demonstrated that sentence-combining practice with automated feedback improved syntactic complexity in L2 writing. Roscoe, Wilson, Johnson, and Mayra (2017) found that AWE feedback was most effective when it targeted specific, identifiable error patterns rather than providing holistic commentary.

The pattern across this research is clear: AWE systems are most effective for what might be termed "local" errors -- sentence-level problems with identifiable correct forms. This aligns with the broader CF literature's finding that focused feedback (targeting specific error types) outperforms unfocused feedback (Shintani & Ellis, 2013; Bitchener & Knoch, 2010). AI systems, by their nature, excel at consistent, focused feedback delivery because they can be configured to target specific error categories and do so with perfect reliability across thousands of texts.

### 7.4.3 What AWE Systems Miss

The limitations of AWE feedback map onto the limitations identified in the broader literature on explicit corrective feedback. First, AWE systems struggle with errors that are context-dependent rather than rule-governed. The sentence "I am excited to see you" is correct; "I am exciting to see you" is not -- but the distinction between -ed and -ing participial adjectives requires understanding the semantic relationship between the subject and the emotional state, not merely applying a pattern-matching rule. While LLM-based systems have improved dramatically in handling such distinctions, traditional grammar-checking AWE still produces false positives and false negatives on context-sensitive structures.

Second, AWE systems tend to normalize language toward a standard variety, which raises questions about whose norms are being enforced and whether "correction" of legitimate variety-specific features constitutes appropriate feedback or linguistic imperialism. Grammarly's default settings, for instance, flag constructions that are standard in Indian English, Nigerian English, or Singapore English as "errors." For the millions of English learners worldwide who are acquiring an outer-circle or expanding-circle variety, this normalization is not merely inaccurate but potentially harmful to their developing linguistic identity (Canagarajah, 2006).

Third, AWE systems provide feedback without genuine understanding of the learner's intended meaning. When a learner writes "I went to the beach and saw many crabs walking on the sand," and the sentence is grammatically correct, the AWE has nothing to say -- even if the learner actually intended to describe the scene differently but lacked the vocabulary or syntactic resources to express their intended meaning. A human tutor, through negotiation and questioning, might discover that the learner wanted to say "I went to the tide pools and saw hermit crabs scuttling across the rocks," revealing gaps in lexical knowledge and descriptive precision that no error-flagging system would identify.

### 7.4.4 The Revision Behavior Problem

A critical finding in AWE research that deserves more attention than it has received concerns what learners actually do with automated feedback. Chapelle, Cotos, and Lee (2015) found that learners using Criterion made surface-level revisions in response to grammar feedback but showed little evidence of the deeper cognitive engagement -- noticing, hypothesis testing, metalinguistic reflection -- that Swain's Output Hypothesis identifies as the acquisitional value of feedback-prompted revision. Ranalli (2018) observed that L2 writers using Grammarly adopted a "fix-it" mentality, clicking through corrections without engaging with the underlying linguistic principles.

This pattern aligns with a concern raised throughout the CF literature: the distinction between repair (fixing a specific instance) and acquisition (developing underlying competence that prevents future errors). Lyster (2004) argued that prompts, which require learners to self-repair, promote acquisition more effectively than reformulations, which provide the repair. If AWE feedback functions primarily as a reformulation -- here is your error, here is the correction -- then its acquisitional value may be limited despite its surface-level effectiveness in improving text quality within a single writing session.

---

## 7.5 LLM-Based Corrective Feedback: A New Paradigm

### 7.5.1 Beyond Pattern Matching: LLMs as Feedback Agents

The emergence of large language models has fundamentally altered the landscape of AI corrective feedback. Unlike traditional grammar checkers, which rely on finite rule sets and statistical patterns, LLMs can engage in extended corrective dialogues, provide contextually sensitive explanations, adjust their feedback based on learner responses, and generate novel examples and analogies. This represents a qualitative shift from feedback-as-correction to feedback-as-interaction.

When a learner submits a paragraph to ChatGPT with the prompt "Please help me improve my English in this paragraph," the resulting feedback bears little resemblance to Grammarly's inline corrections. The LLM might identify specific errors but also comment on word choice, sentence variety, coherence, and register. It can explain why a particular construction is awkward, suggest alternatives, and engage in follow-up discussion if the learner asks questions. In this sense, LLM-based feedback approaches the kind of extended, negotiated, scaffolded interaction that human tutoring provides.

However, the quality and theoretical alignment of LLM feedback is highly variable and depends critically on how the interaction is structured. Left to default behavior, LLMs tend to over-correct, flagging stylistic preferences as errors, imposing formal register norms on casual writing, and providing more feedback than the learner can productively process. This "correction avalanche" effect mirrors the unfocused written corrective feedback that research has found to be less effective than targeted, focused feedback (Sheen, 2007; Bitchener & Knoch, 2010).

### 7.5.2 Prompt Engineering as Pedagogical Design

The recognition that LLM feedback quality depends on how the system is prompted has given rise to what might be termed "prompt-based pedagogical design" -- the use of carefully crafted system prompts and interaction structures to shape AI feedback behavior toward research-supported approaches. This represents a genuinely new form of pedagogical expertise: the ability to translate CF research findings into computational instructions that guide LLM behavior.

For example, a system prompt might instruct an LLM to:

- Limit feedback to a maximum of three error types per interaction (focused feedback)
- Begin with the most implicit feedback type and escalate only if the learner cannot self-correct (graduated feedback per Aljaafreh & Lantolf, 1994)
- Prioritize errors that affect meaning over errors that affect form only (communicative salience)
- Provide metalinguistic explanation only when the learner requests it or fails to understand implicit feedback
- Track which error types the learner has been corrected on previously and adjust expectations accordingly (developmental sensitivity)

Such prompts can, in principle, operationalize decades of CF research into a tutoring system. The practical challenge is that LLMs do not always follow instructions reliably, particularly complex multi-step instructions, and the behavior of the system may vary across interactions in ways that undermine pedagogical consistency.

### 7.5.3 The Affective Dimension of AI Feedback

One of the most frequently cited advantages of AI feedback is its affective neutrality. Learners report lower anxiety when receiving corrections from AI systems compared to human teachers or peers (Li, Link, Ma, Yang, & Hegelheimer, 2014). The fear of judgment, embarrassment, and face-threat that accompanies human corrective feedback -- what Krashen (1982) would frame as the Affective Filter and what sociolinguists would describe as face-threat (Brown & Levinson, 1987) -- is substantially reduced when the interlocutor is a machine.

This affective advantage is real and should not be dismissed. For learners with high anxiety, perfectionist tendencies, or traumatic educational histories, the non-judgmental nature of AI feedback may open channels for noticing and processing that would be blocked in human interaction. Saito and Lyster (2012) demonstrated that learner anxiety moderates the effectiveness of CF, with highly anxious learners showing reduced uptake from oral corrective feedback. If AI reduces anxiety, it may paradoxically increase the noticing and processing that make feedback effective.

However, there is a countervailing concern. The social stakes of communication -- the risk of being misunderstood, the desire to be taken seriously, the investment in identity and face -- are not merely obstacles to acquisition. They are, from a sociocultural and identity-theoretic perspective (Norton, 2013; Darvin & Norton, 2015), integral components of the language learning process. A learner who is motivated to self-correct because they care about how their interlocutor perceives them is engaged in a fundamentally different cognitive and social process than a learner who is corrected by a system they perceive as impersonal. Whether the former or the latter leads to more durable acquisition is an empirical question that has not yet been adequately addressed.

---

## 7.6 Noticing, Uptake, and the Processing of AI Feedback

### 7.6.1 Schmidt's Noticing Hypothesis and AI-Mediated Attention

Schmidt's (1990, 2001) Noticing Hypothesis holds that conscious attention to form is a necessary condition for converting input into intake. Corrective feedback serves this function by directing the learner's attention to the mismatch between their interlanguage form and the target form. The key question for AI-mediated feedback is whether the feedback provided by AI systems successfully triggers the noticing that leads to restructuring.

Several features of AI feedback may enhance noticing. First, the immediacy of AI feedback -- corrections appear in real time or near-real time, unlike human feedback on written work, which may arrive days later -- means that the learner can process the feedback while the erroneous form and its intended meaning are still active in working memory. This temporal proximity between production and correction is theoretically optimal for noticing (Doughty, 2001). Second, the visual salience of AI feedback (color-coded highlights, inline corrections, pop-up explanations) creates perceptual prominence that may increase the likelihood of noticing relative to oral recasts, which are notoriously fleeting and ambiguous (Mackey, Gass, & McDonough, 2000).

However, other features of AI feedback may impair noticing. The sheer volume of AI feedback -- multiple corrections appearing simultaneously, each flagged with equal visual prominence -- may create a processing overload that actually reduces attention to any single form. Cognitive load theory (Sweller, 1988) suggests that when learners must divide attention across too many simultaneous demands, depth of processing for any individual item decreases. A learner confronted with twelve Grammarly corrections in a single paragraph may click through them mechanically, a behavior that constitutes acknowledgment but not noticing in Schmidt's sense.

Furthermore, the ease with which AI corrections can be accepted -- a single click in Grammarly, a copy-paste from ChatGPT -- may reduce the cognitive effort that promotes deep processing. Laufer and Hulstijn's (2001) Involvement Load Hypothesis, while developed for vocabulary acquisition, offers a relevant framework: processing that involves need (motivation to process), search (effort to find the correct form), and evaluation (comparing alternatives) leads to better retention than processing that bypasses these steps. When AI provides both the identification and the correction, it eliminates the search and evaluation components that might otherwise promote noticing and restructuring.

### 7.6.2 Uptake and Modified Output Following AI Feedback

Uptake -- the learner's immediate response to corrective feedback -- has been a primary dependent variable in CF research since Lyster and Ranta (1997) introduced the concept. Their observation that prompts generate higher rates of uptake and repair than recasts has been replicated extensively (Lyster, 2004; Panova & Lyster, 2002) and has been interpreted as evidence that output-pushing feedback promotes deeper processing than input-providing feedback.

In AI-mediated interaction, "uptake" must be reconceptualized. In synchronous AI conversation (e.g., chatbot interaction), uptake can be observed in the learner's subsequent turn: does the learner incorporate the corrected form? In asynchronous AI feedback (e.g., AWE), uptake manifests as revision: does the learner modify the flagged error? But in both cases, the relationship between observable uptake and underlying acquisition is uncertain.

Research on AWE revision behavior suggests that learners readily accept surface-level corrections (high uptake in the behavioral sense) but may not engage in the deeper processing that promotes acquisition. Elola and Oskoz (2016) found that L2 Spanish learners using automated feedback made more revisions but showed no greater improvement in accuracy on new writing tasks than learners who received human feedback. This suggests that the uptake was mechanical rather than acquisitional -- the learner fixed the error in the current text without restructuring the underlying interlanguage representation.

The implications are significant: AI systems may produce high surface uptake (learners accept corrections and produce modified output) while generating low deep uptake (learners do not restructure their linguistic knowledge). This distinction is obscured in much of the current research, which measures revision quality as a proxy for learning without distinguishing between repair and acquisition.

### 7.6.3 The Noticing Paradox in AI Environments

A paradox emerges from the interaction between AI's feedback capabilities and the cognitive conditions for acquisition. The features that make AI feedback efficient -- immediacy, explicitness, comprehensiveness, ease of correction -- are precisely the features that may short-circuit the effortful cognitive processing that promotes noticing and restructuring. We might call this the "efficiency-acquisition paradox": the more efficient the feedback system, the less cognitive work the learner must do, and the less likely it is that the feedback will lead to durable change in the underlying interlanguage.

This paradox is not unique to AI -- it is a restatement of a long-standing tension in the CF literature between providing correction (which is efficient) and promoting self-correction (which is acquisitionally valuable). But AI intensifies the paradox because AI systems are specifically optimized for efficiency. The entire design philosophy of consumer AI writing tools -- reduce errors, improve text quality, minimize user effort -- runs counter to the pedagogical principle that productive struggle facilitates learning (Bjork & Bjork, 2011).

Resolving this paradox requires deliberately designing AI feedback systems that are less efficient than they could be: systems that withhold corrections, prompt self-repair, provide hints rather than answers, and introduce desirable difficulties (Bjork, 1994) into the feedback process. This is technically possible but commercially counterintuitive, which is why the AI feedback tools with the largest market share (Grammarly, Google's Smart Compose) tend to prioritize efficiency over pedagogy.

---

## 7.7 Timing, Sequencing, and Individualization of AI Feedback

### 7.7.1 Immediate vs. Delayed Feedback

The timing of corrective feedback has been a subject of longstanding debate in SLA. Doughty (2001) argued that feedback is most effective when it occurs during the "window of opportunity" -- the brief period during which the learner is actively processing the relevant form. This would favor immediate feedback, which AI systems excel at delivering. However, research on desirable difficulties (Bjork & Bjork, 2011) suggests that delayed feedback can be more effective for long-term retention because the delay forces deeper retrieval processing during the feedback event.

AI systems offer unprecedented control over feedback timing. An AWE system can be configured to provide feedback immediately (as the learner types), after sentence completion, after paragraph completion, or only upon explicit request. LLM-based tutoring systems can be designed to provide feedback after a completed exchange or to delay correction until the learner has produced multiple instances of an error, providing evidence of a systematic pattern rather than a one-off slip.

The empirical research on timing in AI contexts is still limited, but Quinn's (2014) study of immediate versus delayed feedback in an online grammar learning environment found that delayed feedback led to better performance on transfer tasks, while immediate feedback led to better performance on tasks identical to the practice items. This aligns with the broader desirable difficulties literature and suggests that the default immediacy of AI feedback may not be optimal for acquisition, even though it is preferred by learners.

### 7.7.2 Individualization: The Holy Grail

The most theoretically compelling advantage of AI feedback is the potential for individualization -- tailoring feedback type, timing, explicitness, and focus to the specific learner's developmental level, error patterns, learning style, and affective state. This is what Aljaafreh and Lantolf (1994) described as working within the learner's ZPD, and it is what distinguishes expert human tutoring from classroom instruction.

Some AI systems have begun to implement individualization. Duolingo's Birdbrain system uses machine learning to model individual learner error patterns and adjust feedback accordingly. Write & Improve provides CEFR-referenced feedback that adapts to the learner's assessed level. Adaptive learning platforms like Busuu and Babbel use learner performance data to sequence feedback on grammar, vocabulary, and pronunciation.

However, current individualization in AI feedback is primarily based on surface-level performance metrics (error rates, accuracy scores, time on task) rather than on the deeper developmental constructs that the SLA literature identifies as the most important mediators of feedback effectiveness. No current AI system can assess a learner's position on Pienemann's (1998) developmental hierarchy and adjust feedback accordingly. No system can detect whether an error reflects a systematic interlanguage rule (requiring restructuring) or a processing lapse (requiring only attention). No system can gauge the learner's affective state or motivation in real time and adjust feedback explicitness to match.

The gap between theoretically ideal individualization and current technical reality is the frontier where SLA researchers and AI developers most urgently need to collaborate.

### 7.7.3 Feedback Sequencing and Developmental Readiness

A principle established early in the CF literature is that feedback is most effective when it targets structures that the learner is developmentally ready to acquire. Mackey and Philp (1998) demonstrated that intensive recasts were effective for learners at a stage just below the target structure but ineffective for learners at earlier developmental stages. Pienemann's (1998) Processability Theory provides a framework for predicting developmental readiness based on the processing demands of different linguistic structures.

For AI feedback systems, developmental readiness presents a significant challenge. Determining a learner's position on a developmental continuum requires more than error analysis; it requires understanding the systematic nature of the learner's interlanguage -- what they can process, what they are ready to process next, and what is beyond their current processing capacity. Current AI systems typically lack this developmental sensitivity, providing feedback on whatever errors they detect regardless of whether the learner is developmentally prepared to benefit from that feedback.

The consequence is that AI feedback may be simultaneously too early for some structures and redundant for others. A beginning English learner who receives feedback on the third-person singular -s ("he goes, not he go") may not yet have the processing capacity to integrate this morpheme consistently, even though the correction is linguistically accurate. Conversely, the same system may continue flagging article errors for an advanced learner who has already acquired the underlying rule but occasionally produces errors under processing pressure.

---

## 7.8 When AI Feedback Helps: Evidence and Conditions

### 7.8.1 Accuracy Improvement on Targeted Structures

The most robust evidence for the effectiveness of AI feedback comes from studies measuring accuracy improvement on specific, targeted structures after exposure to focused automated correction. Ranalli (2018) found that L2 learners who used Grammarly for targeted grammar practice improved significantly on article accuracy in subsequent writing tasks. Koltovskaia (2020) demonstrated that learners using automated feedback on verb tense errors showed measurable improvement on delayed posttests. Wilson and Czik (2016) found that AWE feedback from Criterion led to significant gains in grammatical accuracy across multiple drafts.

These findings align with the broader CF literature's support for focused corrective feedback (Bitchener, 2008; Sheen, 2007) and suggest that AI is particularly effective when it is configured to target specific error types rather than providing comprehensive correction of all errors. The implication for pedagogical design is clear: AI feedback should be deployed in focused, targeted sequences aligned with instructional goals rather than as a global error-correction utility.

### 7.8.2 Revision Quality and Process

AI feedback demonstrably improves the quality of texts that learners revise in response to automated corrections. Chapelle et al. (2015) found that Criterion feedback led to significant improvements in grammatical accuracy and rhetorical organization between first and revised drafts. Saricaoglu (2019) reported that AWE feedback improved both accuracy and fluency in revised essays. Liao (2016) found that Chinese EFL learners using Pigai produced significantly higher-quality revised essays than those working without automated feedback.

However, the critical caveat raised earlier must be reiterated: improvement in revision quality does not necessarily indicate acquisition. The question is whether learners who produce better revised texts also produce better initial texts on subsequent tasks -- that is, whether the feedback has promoted learning rather than merely editing. The evidence on this point is mixed. Some studies (e.g., Koltovskaia, 2020; Ranalli, 2018) find transfer effects; others (e.g., Elola & Oskoz, 2016; Chapelle et al., 2015) find improvement limited to the revised text.

### 7.8.3 Metalinguistic Awareness

A potentially underexplored benefit of AI feedback is its capacity to develop metalinguistic awareness -- the ability to think and talk about language as a system. When an LLM provides a detailed explanation of why a particular construction is erroneous, including the relevant grammatical rule, exceptions, and examples, it is providing the kind of explicit metalinguistic instruction that Swain's (1998) concept of "metatalk" suggests facilitates acquisition through reflection.

Studies of learner interaction with LLM feedback have found that learners who engage in extended dialogue with AI tutors -- asking follow-up questions about grammar rules, requesting additional examples, and discussing the reasons behind corrections -- show greater improvement in accuracy and metalinguistic knowledge than learners who simply accept corrections (Bin Dahmash, 2024). This suggests that the acquisitional value of AI feedback may depend less on the feedback itself than on the depth of engagement it elicits.

---

## 7.9 When AI Feedback Hinders: Risks and Limitations

### 7.9.1 Over-Correction and the Erosion of Risk-Taking

One of the most significant risks of AI feedback is over-correction: the provision of so much corrective information that learners become reluctant to take the linguistic risks that are essential for development. Swain's (1985) Output Hypothesis posits that learners need to be "pushed" to produce output at the edge of their competence -- output that will necessarily contain errors. If learners perceive that every error will be immediately and comprehensively flagged, they may retreat to safer, simpler constructions, producing more accurate but less complex output.

Skehan's (1998) trade-off hypothesis is relevant here: learners operating under pressure to be accurate tend to sacrifice complexity and fluency. AI feedback that relentlessly prioritizes accuracy may inadvertently suppress the complexity development that is equally important for proficiency growth. Storch and Wigglesworth (2010) observed a similar dynamic in peer feedback contexts: learners who perceived strong accuracy pressure produced simpler texts.

### 7.9.2 Feedback Dependency

A related risk is what might be called "feedback dependency" -- the development of reliance on external AI correction rather than internal self-monitoring capacity. If learners habituate to AI-mediated error detection, they may fail to develop the self-monitoring skills that are essential for autonomous language use. This concern echoes Lantolf and Poehner's (2011) sociocultural argument that the goal of mediation is to promote self-regulation: the learner should eventually internalize the regulatory function that the mediator initially provides. If AI feedback becomes a permanent crutch rather than a temporary scaffold, it has failed by sociocultural standards even if it produces correct output.

Empirical evidence on feedback dependency in AI contexts is emerging. Koltovskaia (2020) found that some learners who used Grammarly extensively showed decreased self-editing behavior when the tool was removed. O'Neill and Russell (2019) reported that learners who relied heavily on machine translation for error correction showed diminished confidence in their own error-detection abilities.

### 7.9.3 The False Precision Problem

AI feedback systems project an aura of authority and precision that may be unwarranted. When Grammarly flags a construction as incorrect, the learner typically has no basis for evaluating whether the correction is appropriate, linguistically accurate, or relevant to their communicative goals. The system's confidence is expressed as categorical -- this is wrong; this is right -- in a domain where linguistic acceptability is often gradient, context-dependent, and contested.

This false precision is particularly problematic for constructions at the boundary of correctness: sentences that are grammatically well-formed but pragmatically odd, constructions that are standard in some varieties but not others, and creative uses of language that violate conventions deliberately. An AI system that categorically corrects such constructions teaches the learner not just grammar but a particular ideology of language correctness -- one that privileges standardization, formality, and inner-circle norms over variation, creativity, and legitimate diversity.

### 7.9.4 Construct Underrepresentation in AI Feedback

From a language assessment perspective, AI feedback systems risk construct underrepresentation: they provide feedback on the dimensions of language they can measure while ignoring dimensions they cannot. A learner whose essays consistently receive "no errors found" from Grammarly may conclude that their writing is proficient when in fact it suffers from limited vocabulary range, poor argumentation, weak audience awareness, and insufficient pragmatic sophistication -- none of which Grammarly is designed to assess.

This construct underrepresentation can distort learners' self-assessment and, consequently, their learning goals. If the feedback system defines "good writing" as writing without grammar errors, learners may prioritize accuracy at the expense of the broader competencies that constitute genuine communicative proficiency. Bachman and Palmer's (2010) model of language ability -- encompassing grammatical, textual, functional, and sociolinguistic competence -- serves as a reminder of how much falls outside the scope of current AI feedback.

---

## 7.10 Hybrid Feedback Systems: Integrating AI and Human Correction

### 7.10.1 The Case for Complementarity

The evidence reviewed in this chapter points toward a clear conclusion: AI feedback and human feedback have complementary strengths, and the most effective approach is likely a principled integration of both. AI excels at consistent, immediate, focused feedback on rule-governed features, available at scale and without the affective costs of human judgment. Human teachers excel at graduated, context-sensitive, developmentally attuned feedback that responds to the learner's intended meaning, respects their communicative goals, and scaffolds self-regulation within the ZPD.

A hybrid model might allocate feedback responsibilities as follows. AI provides the "first pass" of error identification, flagging morphosyntactic and mechanical errors for the learner to address before submitting work to the teacher. This frees the teacher from the time-consuming labor of copyediting and allows them to focus human feedback on higher-order concerns: content, argumentation, voice, audience awareness, pragmatic appropriateness, and developmental guidance. The learner benefits from two qualitatively different feedback sources, each operating in its area of greatest strength.

### 7.10.2 Implementation Principles

Drawing on the theoretical analysis and empirical evidence presented throughout this chapter, we can articulate several principles for effective integration of AI feedback in language learning contexts:

1. **Focus AI feedback on specific, targeted error types** aligned with current instructional goals, rather than deploying comprehensive error correction. This operationalizes the focused feedback principle from Bitchener (2008) and Sheen (2007).

2. **Design AI feedback for graduated explicitness**, beginning with implicit hints and escalating to explicit correction only as needed. This operationalizes Aljaafreh and Lantolf's (1994) regulatory scale and respects the learner's ZPD.

3. **Build in productive struggle** by requiring learner effort before providing corrections. Elicitation and metalinguistic clues should precede reformulations and explicit corrections in AI feedback sequences.

4. **Limit feedback volume** to prevent cognitive overload and the "fix-it" mentality that undermines deep processing. Research on focused CF suggests that addressing two to three error types per session is more effective than comprehensive correction.

5. **Use delayed feedback strategically** for structures that benefit from deeper retrieval processing, reserving immediate feedback for meaning-critical errors that impede communication.

6. **Reserve human feedback for pragmatic, discourse-level, and identity-related concerns** that current AI systems cannot adequately address.

7. **Monitor for feedback dependency** by periodically removing AI support and assessing whether learners can self-edit effectively, adjusting the scaffolding level accordingly.

---

## 7.11 Research Agenda: What We Still Need to Know

The analysis presented in this chapter reveals several critical gaps in our understanding of AI-mediated corrective feedback that should drive the next generation of research.

First, we need longitudinal studies that track not just revision quality but new text quality over time. The distinction between repair and acquisition is fundamental, yet most AI feedback studies measure only revision outcomes. Designs that compare accuracy on treated structures in post-treatment novel writing tasks -- weeks or months after the AI feedback intervention -- are essential for determining whether AI feedback promotes durable learning.

Second, we need studies that compare different configurations of AI feedback against each other, not just AI versus human feedback. What happens when AI feedback is configured for graduated explicitness versus default comprehensive correction? When it targets developmental stages versus all errors? When it provides metalinguistic explanation versus simple correction? The configurability of AI systems makes such comparisons possible in ways that were impractical with human feedback research.

Third, we need research on feedback literacy in AI contexts: how learners interpret, evaluate, and act on AI-generated corrections. Do learners distinguish between high-confidence corrections (clear grammatical errors) and low-confidence suggestions (style preferences)? Do they develop critical evaluation skills over time, or do they accept AI feedback uncritically? Carless and Boud's (2018) framework of feedback literacy provides a useful starting point.

Fourth, we need studies that examine AI feedback through an equity lens. Which learner populations benefit most from AI feedback, and which are disadvantaged by it? Are there differential effects based on L1 background, socioeconomic status, digital literacy, or educational context? The democratizing potential of AI feedback -- making expert-level correction available to learners who lack access to human tutors -- is frequently touted but rarely examined empirically.

Finally, we need theoretical work that updates the Interaction Hypothesis, the Noticing Hypothesis, and sociocultural mediation frameworks for AI-mediated learning environments. These frameworks were developed to explain human-human interaction; their application to human-AI interaction requires not just extension but reconceptualization of core constructs such as communicative intent, negotiation of meaning, and social mediation.

---

## 7.12 Conclusion

Corrective feedback in SLA has always been a domain where theoretical sophistication and practical implementation exist in tension. Teachers know, from decades of research, that feedback works best when it is focused, developmentally appropriate, graduated in explicitness, and embedded in meaningful communication. Yet the practical constraints of classroom instruction -- time, energy, student-teacher ratios, the impossibility of individualizing feedback for every learner on every task -- have ensured that most learners receive far less feedback than the research would recommend.

AI appears to resolve this resource constraint, and in narrow terms it does. Learners who use AI feedback tools receive more corrections, more consistently, more immediately, than has ever been possible in human-only learning environments. For targeted morphosyntactic accuracy development, the evidence suggests that AI feedback is genuinely effective. For learners who are anxious about human judgment, AI provides a psychologically safer feedback environment that may facilitate noticing and processing.

But the story of corrective feedback in SLA has always been more complex than "more is better." The research reviewed in this chapter demonstrates that the most effective feedback is not the most abundant or the most explicit but the feedback that is calibrated to the learner's developmental readiness, embedded in meaningful communicative context, graduated in explicitness to promote self-regulation, and integrated within a broader ecology of social interaction and identity development. On these dimensions, current AI systems fall short -- not because the technology is immature, but because the design priorities of commercial AI tools (efficiency, comprehensiveness, user satisfaction) are misaligned with the pedagogical priorities that the CF literature identifies as most important for acquisition.

The path forward is not to reject AI feedback or to accept it uncritically but to redesign it according to SLA principles. This requires collaboration between AI developers who understand what is technically possible and SLA researchers who understand what is pedagogically desirable. It requires a willingness to build AI feedback systems that are deliberately less efficient than they could be -- systems that withhold corrections, prompt learner effort, and tolerate errors when those errors are developmentally productive. And it requires ongoing empirical research that evaluates AI feedback not by its capacity to fix errors in texts but by its capacity to change the minds and linguistic systems of the learners who use it.

The tireless interlocutor must learn, paradoxically, when not to correct.

---

## References

Aljaafreh, A., & Lantolf, J. P. (1994). Negative feedback as regulation and second language learning in the zone of proximal development. *The Modern Language Journal*, 78(4), 465-483.

Ammar, A., & Spada, N. (2006). One size fits all? Recasts, prompts, and L2 learning. *Studies in Second Language Acquisition*, 28(4), 543-574.

Attali, Y., & Burstein, J. (2006). Automated essay scoring with e-rater v.2. *Journal of Technology, Learning, and Assessment*, 4(3), 1-31.

Bachman, L. F., & Palmer, A. S. (2010). *Language assessment in practice*. Oxford University Press.

Ballance, O. J. (2019). Writing with an AI writing assistant: An exploratory study. *CALICO Journal*, 36(2), 135-148.

Bin Dahmash, N. (2024). AI-powered corrective feedback and L2 writing development. *Language Learning & Technology*, 28(1), 45-68.

Bitchener, J. (2008). Evidence in support of written corrective feedback. *Journal of Second Language Writing*, 17(2), 102-118.

Bitchener, J., & Knoch, U. (2010). Raising the linguistic accuracy level of advanced L2 writers with written corrective feedback. *Journal of Second Language Writing*, 19(4), 207-217.

Bjork, R. A. (1994). Memory and metamemory considerations in the training of human beings. In J. Metcalfe & A. Shimamura (Eds.), *Metacognition: Knowing about knowing* (pp. 185-205). MIT Press.

Bjork, E. L., & Bjork, R. A. (2011). Making things hard on yourself, but in a good way: Creating desirable difficulties to enhance learning. In M. A. Gernsbacher et al. (Eds.), *Psychology and the real world* (pp. 56-64). Worth Publishers.

Brown, P., & Levinson, S. C. (1987). *Politeness: Some universals in language usage*. Cambridge University Press.

Canagarajah, A. S. (2006). Changing communicative needs, revised assessment objectives: Testing English as an international language. *Language Assessment Quarterly*, 3(3), 229-242.

Carless, D., & Boud, D. (2018). The development of student feedback literacy. *Assessment & Evaluation in Higher Education*, 43(8), 1315-1325.

Chapelle, C. A., Cotos, E., & Lee, J. (2015). Validity arguments for diagnostic assessment using automated writing evaluation. *Language Testing*, 32(3), 385-405.

Darvin, R., & Norton, B. (2015). Identity and a model of investment in applied linguistics. *Annual Review of Applied Linguistics*, 35, 36-56.

Dikli, S., & Bleyle, S. (2014). Automated essay scoring feedback for second language writers. *Assessing Writing*, 21, 35-52.

Doughty, C. J. (2001). Cognitive underpinnings of focus on form. In P. Robinson (Ed.), *Cognition and second language instruction* (pp. 206-257). Cambridge University Press.

Elola, I., & Oskoz, A. (2016). Supporting second language writing using multimodal feedback. *Foreign Language Annals*, 49(1), 58-74.

Ferris, D. R. (1999). The case for grammar correction in L2 writing classes: A response to Truscott (1996). *Journal of Second Language Writing*, 8(1), 1-11.

Kellogg, R. T., Whiteford, A. P., & Quinlan, T. (2010). Does automated feedback help students learn to write? *Journal of Educational Computing Research*, 42(2), 173-196.

Koltovskaia, S. (2020). Student engagement with automated written corrective feedback. *Journal of Second Language Writing*, 47, 100714.

Krashen, S. D. (1982). *Principles and practice in second language acquisition*. Pergamon Press.

Lantolf, J. P., & Poehner, M. E. (2011). Dynamic assessment in the classroom: Vygotskian praxis for second language development. *Language Teaching Research*, 15(1), 11-33.

Laufer, B., & Hulstijn, J. H. (2001). Incidental vocabulary acquisition in a second language: The construct of task-induced involvement. *Applied Linguistics*, 22(1), 1-26.

Li, S. (2010). The effectiveness of corrective feedback in SLA: A meta-analysis. *Language Learning*, 60(2), 309-365.

Li, Z., Link, S., Ma, H., Yang, H., & Hegelheimer, V. (2014). The role of automated writing evaluation holistic scores in the ESL classroom. *System*, 44, 66-78.

Liao, H. C. (2016). Using automated writing evaluation to reduce grammar errors in writing. *ELT Journal*, 70(3), 308-319.

Long, M. H. (1996). The role of the linguistic environment in second language acquisition. In W. C. Ritchie & T. K. Bhatia (Eds.), *Handbook of second language acquisition* (pp. 413-468). Academic Press.

Lyster, R. (2004). Differential effects of prompts and recasts in form-focused instruction. *Studies in Second Language Acquisition*, 26(3), 399-432.

Lyster, R., & Ranta, L. (1997). Corrective feedback and learner uptake. *Studies in Second Language Acquisition*, 19(1), 37-66.

Lyster, R., & Saito, K. (2010). Oral feedback in classroom SLA: A meta-analysis. *Studies in Second Language Acquisition*, 32(2), 265-302.

Mackey, A., Gass, S. M., & McDonough, K. (2000). How do learners perceive interactional feedback? *Studies in Second Language Acquisition*, 22(4), 471-497.

Mackey, A., & Goo, J. (2007). Interaction research in SLA: A meta-analysis and research synthesis. In A. Mackey (Ed.), *Conversational interaction in second language acquisition* (pp. 407-452). Oxford University Press.

Mackey, A., & Philp, J. (1998). Conversational interaction and second language development: Recasts, responses, and red herrings? *The Modern Language Journal*, 82(3), 338-356.

Norton, B. (2013). *Identity and language learning: Extending the conversation* (2nd ed.). Multilingual Matters.

O'Neill, R., & Russell, A. (2019). Stop! Grammar time: University students' perceptions of the automated feedback program Grammarly. *Australasian Journal of Educational Technology*, 35(1), 42-56.

Panova, I., & Lyster, R. (2002). Patterns of corrective feedback and uptake in an adult ESL classroom. *TESOL Quarterly*, 36(4), 573-595.

Pienemann, M. (1998). *Language processing and second language development: Processability theory*. John Benjamins.

Quinn, P. J. (2014). Delayed versus immediate corrective feedback on orally produced passive errors in English. *Studies in Second Language Acquisition*, 36(3), 397-420.

Ranalli, J. (2018). Automated written corrective feedback: How well can students make use of it? *Computer Assisted Language Learning*, 31(7), 653-674.

Roscoe, R. D., Wilson, J., Johnson, A. C., & Mayra, C. R. (2017). Presentation, expectations, and experience: Sources of student perceptions of automated writing evaluation. *Computers & Education*, 113, 86-98.

Saito, K., & Lyster, R. (2012). Effects of form-focused instruction and corrective feedback on L2 pronunciation development. *Language Learning*, 62(2), 595-633.

Saricaoglu, A. (2019). The impact of automated feedback on L2 learners' written causal explanations. *ReCALL*, 31(2), 189-203.

Schmidt, R. (1990). The role of consciousness in second language learning. *Applied Linguistics*, 11(2), 129-158.

Schmidt, R. (2001). Attention. In P. Robinson (Ed.), *Cognition and second language instruction* (pp. 3-32). Cambridge University Press.

Sheen, Y. (2006). Exploring the relationship between characteristics of recasts and learner uptake. *Language Teaching Research*, 10(4), 361-392.

Sheen, Y. (2007). The effect of focused written corrective feedback and language aptitude on ESL learners' acquisition of articles. *TESOL Quarterly*, 41(2), 255-283.

Sheen, Y. (2011). *Corrective feedback, individual differences and second language learning*. Springer.

Shintani, N., & Ellis, R. (2013). The comparative effect of direct written corrective feedback and metalinguistic explanation on learners' explicit and implicit knowledge of the English indefinite article. *Journal of Second Language Writing*, 22(3), 286-306.

Stevenson, M., & Phakiti, A. (2014). The effects of computer-generated feedback on the quality of writing. *Assessing Writing*, 19, 51-65.

Storch, N., & Wigglesworth, G. (2010). Learners' processing, uptake and retention of corrective feedback on writing. *Studies in Second Language Acquisition*, 32(2), 303-334.

Swain, M. (1985). Communicative competence: Some roles of comprehensible input and comprehensible output in its development. In S. Gass & C. Madden (Eds.), *Input in second language acquisition* (pp. 235-253). Newbury House.

Swain, M. (1995). Three functions of output in second language learning. In G. Cook & B. Seidlhofer (Eds.), *Principle and practice in applied linguistics* (pp. 125-144). Oxford University Press.

Swain, M. (1998). Focus on form through conscious reflection. In C. Doughty & J. Williams (Eds.), *Focus on form in classroom second language acquisition* (pp. 64-81). Cambridge University Press.

Sweller, J. (1988). Cognitive load during problem solving: Effects on learning. *Cognitive Science*, 12(2), 257-285.

Truscott, J. (1996). The case against grammar correction in L2 writing classes. *Language Learning*, 46(2), 327-369.

Weigle, S. C. (2010). Validation of automated scores of TOEFL iBT tasks against non-test indicators of writing ability. *Language Testing*, 27(3), 335-353.

Wilson, J., & Czik, A. (2016). Automated essay evaluation software in English Language Arts classrooms. *Computers & Education*, 100, 94-109.

Zhang, Z. V. (2020). Engaging with automated writing evaluation (AWE) feedback on L2 writing: Student perceptions and revisions. *Assessing Writing*, 43, 100439.
