# Chapter 9: Grammar, Syntax, and Intelligent Tutoring

## Pattern Matching, Rule Knowledge, and the Developmental Question

---

## 9.1 Introduction: The Grammar Problem in the AI Age

Grammar instruction in second language acquisition has been, for more than half a century, the field's most persistent source of theoretical controversy. The pendulum has swung from the audiolingual drills of the 1960s, through the communicative revolution's de-emphasis of explicit grammar teaching in the 1970s and 1980s, to the principled reintegration of form-focused instruction in the 1990s and 2000s, and finally to the current moment in which AI systems offer to deliver grammar instruction that is simultaneously more explicit than any textbook and more communicatively embedded than any task-based syllabus. At each swing of this pendulum, the fundamental questions have remained: Does explicit grammar instruction promote acquisition? If so, what kind, for whom, and when?

These are not merely pedagogical questions. They sit at the intersection of the field's deepest theoretical divides: the interface debate (can explicit knowledge become implicit knowledge?), the teachability problem (are some structures unteachable at certain developmental stages?), the role of consciousness in learning (must learners be aware of a rule to acquire it?), and the relationship between comprehension-based and production-based learning (does understanding a rule translate into ability to use it?). Any technology that claims to "teach grammar" must be evaluated against these theoretical dimensions, not merely against surface-level accuracy metrics.

Artificial intelligence has entered the grammar instruction space through multiple vectors. Traditional grammar checkers (Grammarly, LanguageTool, ProWritingAid) flag rule violations and offer corrections. Intelligent tutoring systems (ITS) diagnose learner errors, model learner knowledge, and adapt instruction accordingly. Large language models explain grammatical rules with unprecedented fluency, generate contextually varied examples, and engage learners in dialogues about form-meaning connections. Adaptive exercise platforms (Duolingo, Babbel, Busuu) sequence grammar instruction based on learner performance data.

This chapter evaluates these AI grammar tools against the theoretical and empirical frameworks that have shaped grammar instruction research in SLA. It begins with Pienemann's Processability Theory and the developmental sequences that constrain what can be taught when, examines DeKeyser's Skill Acquisition Theory and its implications for the explicit-to-implicit knowledge transition, reviews the intelligent tutoring system literature, analyzes how LLMs handle grammar, explores the relationship between AI and both explicit and implicit grammar instruction, and concludes with VanPatten's Processing Instruction as a framework for principled AI grammar design.

---

## 9.2 Processability Theory and Developmental Sequences

### 9.2.1 Pienemann's Framework

Pienemann's (1998, 2005) Processability Theory (PT) proposes that the acquisition of grammatical structures follows a predictable developmental sequence determined by the processing demands of different structures. Learners can only acquire structures for which they have developed the necessary processing prerequisites, regardless of the instructional input they receive. The sequence progresses from structures requiring only lemma access (single words), through category procedures (lexical morphology), phrasal procedures (phrase-level agreement), inter-phrasal procedures (cross-phrasal operations like subject-verb agreement), and finally subordinate clause procedures.

For English, the developmental sequence for question formation illustrates the theory: learners progress from single-word questions ("Coffee?") to canonical word-order questions with rising intonation ("You want coffee?"), to fronted wh-questions without inversion ("Where you go?"), to yes/no inversion ("Can I have coffee?"), to wh-inversion ("Where did you go?"), and finally to embedded questions ("I wonder where he went"). This sequence has been documented in multiple studies across different L1 backgrounds (Pienemann, 1998; Keating & Jegerski, 2015).

The Teachability Hypothesis, which follows from PT, states that instruction can only promote acquisition when the learner is at a stage where they are developmentally ready for the target structure -- that is, when they have acquired the processing prerequisites. Instruction targeting structures beyond the learner's current stage will be ineffective, not because the instruction is poor but because the learner lacks the processing machinery to integrate the new structure into their developing system. Conversely, instruction targeting structures at the next developmental stage -- what Pienemann called the "teachable" structures -- can accelerate acquisition by providing the focused input and practice needed to trigger the transition.

### 9.2.2 Implications for AI Grammar Instruction

Processability Theory presents a fundamental challenge for AI grammar instruction that most current systems have not addressed. The vast majority of AI grammar tools sequence instruction based on one or more of the following criteria: (a) perceived difficulty, as estimated by instructional designers; (b) textbook convention (present tense before past tense, articles before relative clauses); (c) error frequency in the learner's production; or (d) performance on diagnostic tests that measure accuracy but not processability stage.

None of these criteria correspond to the developmental readiness that PT identifies as the critical variable. A learner who makes frequent errors with third-person singular -s may be doing so not because they "don't know the rule" but because they have not yet developed the inter-phrasal processing capacity required to implement subject-verb agreement consistently. Drilling the rule harder, providing more examples, or offering more explicit explanation will not help if the processing prerequisite has not been met. What the learner needs is not more instruction on the target structure but opportunities to consolidate the processing capacity at their current stage before attempting the next.

Implementing PT-informed sequencing in AI grammar systems would require diagnostic assessment of the learner's processability stage -- not just their accuracy on specific structures but the processing operations they can perform. This is technically possible using methods adapted from PT research (e.g., elicited imitation tasks, emergent structure analysis) but has not been implemented in any commercial AI grammar tool to date. The result is that AI grammar instruction often targets structures the learner is not ready to acquire, producing the appearance of learning (correct performance in controlled exercises) without genuine acquisition (consistent use in spontaneous production).

### 9.2.3 Developmental Sequences Beyond PT

Processability Theory is not the only framework that identifies developmental constraints on grammar acquisition. Research on acquisition orders -- the observation that certain morphemes and structures are acquired in a relatively fixed order regardless of L1, instruction, or exposure conditions -- extends back to Dulay and Burt (1974) and Brown (1973) for L1 acquisition. Krashen's (1977) "natural order" hypothesis, based on morpheme acquisition studies, proposed that L2 morphemes are acquired in a predictable order similar (though not identical) to the L1 order.

While the strong version of the natural order hypothesis has been challenged on methodological grounds (Goldschneider & DeKeyser, 2001), the broader finding that certain structures are consistently acquired before others is well-established. Plural -s before third-person -s, progressive -ing before past -ed, copula *be* before auxiliary *be* -- these patterns reflect underlying processing, semantic, and distributional factors that constrain the order of acquisition.

For AI grammar instruction, these developmental findings suggest that the common practice of organizing grammar instruction by "difficulty level" (as rated by textbook authors or NLP error classifiers) may be misaligned with the natural acquisition process. An AI system that drills article usage to a beginning learner -- articles being notoriously late-acquired for speakers of article-less L1s -- is targeting a structure that the learner's developing system may not yet be able to integrate, regardless of how well the AI teaches the rule.

---

## 9.3 Skill Acquisition Theory and Grammar Learning

### 9.3.1 DeKeyser's Framework

DeKeyser's (2007, 2015) Skill Acquisition Theory (SAT), adapted from Anderson's (1993) ACT-R model of cognitive skill development, provides a framework for understanding how grammatical knowledge develops from initial explicit understanding through practice to automatized use. The theory proposes three stages:

1. **Declarative stage**: The learner acquires explicit knowledge of a grammatical rule ("In English, the verb takes -s in the third person singular present tense"). This knowledge is conscious, verbalizable, and accessible through controlled processing.

2. **Procedural stage**: Through practice, the learner begins to apply the rule in real-time production without consciously accessing the declarative representation. The rule is "compiled" into production rules (if-then sequences) that fire automatically in relevant contexts.

3. **Automatic stage**: Through extensive practice, the proceduralized rule becomes fully automatized, requiring minimal attentional resources and operating at speed comparable to native-speaker performance.

The critical mechanism driving progression through these stages is practice -- specifically, the kind of practice that is initially controlled and deliberate (applying the rule consciously) and gradually becomes more spontaneous and communicative (using the structure in meaningful contexts without conscious rule application). DeKeyser (2007) emphasizes that the practice must be meaningful and contextualized; mechanical drill that does not engage the learner in genuine form-meaning mapping does not promote proceduralization.

### 9.3.2 SAT and the Interface Debate

Skill Acquisition Theory takes a strong position on the interface debate -- the question of whether explicit knowledge can become implicit knowledge. The strong interface position, which SAT represents, holds that explicit knowledge can and does become implicit through the declarative-procedural-automatic progression described above. This is precisely what happens, SAT argues, when a learner who initially applies a grammar rule consciously eventually produces the correct form automatically, without awareness of the rule.

The opposing positions -- the non-interface position (Krashen, 1981; Paradis, 2009), which holds that explicit and implicit knowledge are stored in separate systems and that explicit knowledge cannot become implicit, and the weak interface position (R. Ellis, 2005), which holds that explicit knowledge facilitates implicit knowledge through processes like noticing but does not directly convert into it -- have different implications for AI grammar instruction.

If SAT is correct, then AI systems that teach explicit grammar rules and provide extensive practice opportunities for applying those rules in increasingly communicative contexts are facilitating genuine acquisition. The AI's role is to provide the declarative input (clear rule explanation) followed by graduated practice (controlled exercises, then freer production, then spontaneous use) that drives proceduralization.

If the non-interface position is correct, then explicit grammar teaching of any kind -- whether by AI or human -- does not contribute to acquisition; it only develops a monitor that can edit output after the fact. Acquisition, on this view, comes only from meaningful interaction with comprehensible input. AI's role would be limited to providing rich, comprehensible input and interactional opportunities, not grammar instruction per se.

If the weak interface position is correct, then AI grammar teaching contributes to acquisition not directly but by facilitating noticing -- drawing the learner's attention to form-meaning connections in the input so that the implicit acquisition mechanism can operate on them. AI's role would be to enhance input salience and create conditions for noticing, not to teach rules for direct application.

The empirical evidence provides some support for all three positions, which is why the interface debate remains unresolved. However, the weight of evidence from instructed SLA research (Norris & Ortega, 2000; Spada & Tomita, 2010) suggests that explicit instruction does facilitate acquisition, at least for certain structures and certain learners, supporting either the strong or weak interface position and justifying AI grammar instruction as a legitimate component of a comprehensive language learning program.

### 9.3.3 Practice Design for AI Grammar Systems

If SAT provides the correct account of grammar learning, then the design of practice activities in AI grammar systems is critically important. DeKeyser (2007) specified several characteristics of effective practice:

**Meaningful practice**: Exercises must require the learner to process form-meaning connections, not merely manipulate forms. "Fill in the blank with the correct form of the verb" is less meaningful than "Read the paragraph and choose the correct verb form based on when the events occurred." The latter requires temporal reasoning, while the former can be completed by pattern matching alone.

**Graduated complexity**: Practice should progress from controlled activities (where the target structure is the primary focus) through guided activities (where the structure must be used in the context of a broader communicative task) to free activities (where the learner uses the structure spontaneously in unrehearsed communication).

**Sufficient volume**: Proceduralization requires extensive practice -- far more than most language courses provide. DeKeyser (2007) estimated that achieving automaticity on a grammar structure might require thousands of meaningful encounters and productions, a volume that classroom instruction alone cannot provide but that AI-mediated practice theoretically can.

**Varied contexts**: Practice in varied contexts promotes the kind of generalization that characterizes genuine proceduralization, as opposed to the context-specific performance that results from practicing in a single context.

AI grammar systems are well-positioned to provide the volume and variety of practice that SAT recommends, but most current systems fall short on meaningfulness and graduated complexity. Duolingo's grammar exercises, for example, provide high volume and some variety but are largely mechanical (translate this sentence, fill in this blank) rather than genuinely meaningful. LLM-based grammar practice has the potential to be more communicatively meaningful, but only if the interaction is designed to require genuine form-meaning processing rather than mere form manipulation.

---

## 9.4 Intelligent Tutoring Systems for Grammar

### 9.4.1 The ICALL Tradition

Intelligent Computer-Assisted Language Learning (ICALL), a subfield of the broader Intelligent Tutoring Systems (ITS) tradition, has a research history extending back to the 1990s, well before the current AI era. The defining feature of ICALL systems, as distinct from generic CALL, is the use of computational models of language and learner knowledge to provide adaptive, individualized instruction.

Key early ICALL systems include:

**E-Tutor** (Heift, 2001, 2010), developed for German grammar instruction, used NLP to parse learner input, diagnose errors, and provide targeted metalinguistic feedback. E-Tutor could identify the source of an error (morphological, syntactic, lexical) and provide graduated feedback from implicit (highlighting the location of the error) to explicit (explaining the relevant rule). Heift's research demonstrated that learners using E-Tutor showed significant improvement on grammar tests compared to control groups using non-adaptive CALL materials.

**Robo-Sensei** (Nagata, 2009), designed for Japanese grammar instruction, used a parser that could analyze learner input, identify errors related to Japanese-specific grammatical features (particles, verb conjugation, honorifics), and provide feedback calibrated to the error type. Nagata's research found that metalinguistic feedback from the system led to greater accuracy gains than simple error flagging.

**The TAGARELA system** (Amaral & Meurers, 2011) for Portuguese used detailed linguistic analysis to provide feedback on learner production in the context of communicative activities. TAGARELA represented an advance in integrating ICALL feedback with meaningful communication rather than decontextualized grammar exercises.

### 9.4.2 The Architecture of Grammar ITS

Intelligent tutoring systems for grammar typically incorporate four components (Nkambou, Bourdeau, & Mizoguchi, 2010):

**The domain model** encodes knowledge of the target language grammar -- rules, patterns, exceptions, and the relationships among structures. In traditional ICALL, this was typically a hand-crafted grammar; in LLM-based systems, grammatical knowledge is implicit in the model's parameters.

**The student model** tracks the learner's current grammatical knowledge, including what they know, what they are learning, and what they do not yet know. The student model informs decisions about what to teach next, how to provide feedback, and when to advance to new material. The quality of the student model is the primary determinant of an ITS's adaptive capability.

**The tutoring model** (or pedagogical model) encodes the instructional strategy -- how to present new material, when to practice, what kind of feedback to provide, and how to respond to learner errors. In theory, the tutoring model should be informed by SLA research on grammar instruction; in practice, it is often based on intuition, expert judgment, or generic instructional design principles rather than empirically validated SLA theory.

**The user interface** determines how the learner interacts with the system -- text input, multiple choice, drag-and-drop, speech, or conversation.

### 9.4.3 From Rule-Based to Neural: The Architecture Shift

The transition from traditional ICALL to LLM-based grammar tutoring represents a fundamental architectural shift. Traditional ICALL systems used explicit, hand-crafted grammars and parsers to analyze learner input. This approach had the advantage of transparency -- the system could explain exactly why it flagged an error, because the error was identified by reference to an explicit rule -- but the disadvantage of brittleness. Hand-crafted grammars could not handle the full range of learner interlanguage, producing both false positives (flagging correct constructions that the grammar did not anticipate) and false negatives (missing errors outside the grammar's scope).

LLM-based systems invert this architecture. Instead of explicit rules, they rely on statistical patterns learned from massive corpora. This approach handles the full range of language input (including non-standard, interlanguage forms) with remarkable robustness but sacrifices transparency. When an LLM identifies an error, it cannot explain its reasoning in the same way a rule-based system can -- it can generate an explanation (which may be accurate, plausible, or hallucinated), but the explanation is a post-hoc rationalization of a statistical pattern, not a trace of the system's actual processing.

This shift has implications for the quality of grammatical feedback. Rule-based systems provide feedback grounded in explicit grammatical knowledge; LLM-based systems provide feedback grounded in distributional statistics. For well-attested, high-frequency constructions, these converge: both the rule-based and statistical system will correctly identify "He go to school" as an error and flag the missing -s. But for rarer, more complex, or more context-dependent constructions -- the conditional perfect in counterfactual hypotheticals, the subjunctive in formal mandative clauses, the distinction between restrictive and non-restrictive relative clauses -- the LLM's statistical foundation may produce less reliable feedback than a carefully crafted rule-based system.

---

## 9.5 How LLMs Handle Grammar: Pattern Matching vs. Rule Knowledge

### 9.5.1 The Competence Question

A question that has occupied computational linguists, cognitive scientists, and philosophers of mind since the emergence of LLMs is whether these systems possess genuine grammatical knowledge or merely simulate it through sophisticated pattern matching. The question echoes Chomsky's (1965) distinction between competence (the underlying knowledge of language) and performance (the actual use of language in concrete situations). Does an LLM that consistently produces grammatically correct English "know" English grammar in any meaningful sense?

The evidence is complex. Linzen and Baroni (2021) demonstrated that transformer-based models can handle long-distance subject-verb agreement ("The keys to the cabinet *are* on the table") with high accuracy, suggesting sensitivity to hierarchical syntactic structure rather than mere linear proximity. Wilcox, Levy, Morita, and Futrell (2018) found that neural language models assign higher probability to grammatically correct sentences than to minimally different ungrammatical sentences across a range of construction types, including those requiring hierarchical analysis (e.g., center-embedded clauses).

However, other studies have identified systematic failures. Gulordava, Baroni, and Boleda (2018) found that while LLMs handle agreement well in typical sentences, their performance degrades on sentences with unusual structural properties (garden-path sentences, double center-embeddings). McCoy, Frank, and Linzen (2020) demonstrated that models trained on simple heuristics (e.g., "the first noun is the subject") could mimic competence on standard sentences but fail on sentences designed to distinguish structural knowledge from heuristic shortcutting.

For grammar instruction, this matters because an AI grammar tutor that relies on pattern matching rather than genuine rule knowledge may provide correct feedback on typical sentences but incorrect or misleading feedback on atypical ones. A learner who asks, "Is this sentence correct?" and receives an AI response based on distributional probability rather than grammatical analysis may be led astray precisely when they most need guidance -- on the difficult, ambiguous, or unusual constructions that test the boundaries of a rule.

### 9.5.2 Grammatical Explanation as Rationalization

When an LLM explains a grammar rule, it is generating text that conforms to the patterns of grammatical explanation found in its training data. This is different from retrieving the rule that it used to process the sentence. Consider a learner who writes "If I would have known, I would have come" and asks the LLM to explain the error. The LLM might respond: "In standard English, the condition clause of a past counterfactual uses the past perfect, not 'would have.' The correct form is 'If I had known, I would have come.'"

This explanation is accurate, well-formed, and pedagogically useful. But it was not generated by the same mechanism that identified the error. The error was identified by a statistical process that determined the input was unlikely relative to the training distribution; the explanation was generated by a different statistical process that produced text consistent with grammatical metalanguage in the training data. The two processes are independent -- which means that the explanation might be wrong even when the error identification is correct, and vice versa.

Researchers have documented instances of LLMs providing fluent, confident, and incorrect grammatical explanations (Dentella, Raffaelli, & Caglio, 2023). The problem is particularly acute for complex or contested grammatical points where the training data contains conflicting information (e.g., the split infinitive, the sentence-final preposition, the use of "they" as a singular pronoun). On such points, the LLM may produce an explanation that reflects prescriptivist tradition, descriptive linguistics, or a hybrid, depending on the statistical patterns in its training data, without any mechanism for determining which perspective is appropriate for the learner's context.

### 9.5.3 Grammar Across Languages: The Resource Gap

LLM grammatical capabilities vary dramatically across languages, reflecting the distribution of training data. For English, the most extensively represented language in LLM training corpora, grammatical capabilities are strong across a wide range of construction types. For major European languages (French, German, Spanish), capabilities are robust for common structures but less reliable for complex or colloquial constructions. For less-resourced languages (Turkish, Swahili, Tagalog, indigenous languages), grammatical capabilities are substantially weaker, and the risk of incorrect feedback is correspondingly higher.

This resource disparity means that AI grammar instruction reinforces existing inequities in language education. Learners of English have access to highly capable AI grammar tools; learners of Quechua or Yoruba do not. The same technology that promises to democratize language education may, in practice, widen the gap between well-resourced and under-resourced languages.

---

## 9.6 Explicit Grammar Instruction via AI

### 9.6.1 The Case for Explicit Instruction

The meta-analytic evidence on explicit grammar instruction in SLA is clear: explicit instruction produces measurable improvement in both explicit and implicit knowledge of targeted structures, with effects that are durable over time (Norris & Ortega, 2000; Spada & Tomita, 2010). Norris and Ortega's (2000) landmark meta-analysis found that explicit instruction (which includes both deductive rule presentation and inductive consciousness-raising) produced large effect sizes (d = 1.13 on immediate measures, d = 0.96 on delayed measures) compared to implicit instruction or no instruction.

However, these findings come with important qualifications. First, the advantage for explicit instruction is larger on explicit knowledge measures (grammaticality judgments, controlled production) than on implicit knowledge measures (spontaneous production, timed performance), suggesting that explicit instruction may develop explicit knowledge more effectively than implicit knowledge. Second, the advantage varies by structure type: structures with clear, stable rules (e.g., English simple past -ed) benefit more from explicit instruction than structures with complex, variable rules (e.g., English article system). Third, the advantage varies by learner: adults benefit more from explicit instruction than children, and analytic learners benefit more than holistic learners (Erlam, 2005).

### 9.6.2 What AI Does Well: Rule Presentation and Explanation

AI systems -- particularly LLMs -- are remarkably effective at presenting grammatical rules clearly, accurately, and accessibly. An LLM can explain the English present perfect to a learner in multiple ways:

- Deductively: "The present perfect is formed with have/has + past participle and is used for actions that started in the past and continue to the present, or for past actions with present relevance."
- Inductively: presenting multiple examples and asking the learner to identify the pattern
- Contrastively: comparing with the learner's L1 ("In Spanish, you would use the *preterito perfecto compuesto*: *he comido*. The English present perfect works similarly but is used somewhat differently...")
- Through graduated examples: beginning with clear, prototypical uses and progressively introducing more nuanced or atypical applications

This explanatory flexibility surpasses what most textbooks provide and approaches what an expert grammar teacher could offer. The AI can also adjust its explanation in response to learner questions, provide additional examples on request, and rephrase explanations that the learner finds confusing.

### 9.6.3 What AI Struggles With: The Form-Meaning Connection

The limitation of AI explicit instruction lies not in rule presentation but in form-meaning connection. Effective grammar instruction does not merely teach rules; it helps learners connect grammatical forms to the meanings they express. Long's (1991) distinction between *focus on form* (drawing attention to form within a communicative context, where the primary focus is on meaning) and *focus on forms* (teaching grammatical forms as objects of study, outside of communicative context) is critical here.

Most AI grammar instruction defaults to focus on forms: the grammar point is the explicit topic of the exercise or explanation, and the learner's attention is directed to form rather than meaning. This is the approach of grammar checker feedback ("You need the past tense here"), textbook-style exercises ("Choose the correct form"), and even LLM grammar explanations ("Let me explain when to use the present perfect").

Focus on form, by contrast, occurs when the learner encounters a grammatical issue while primarily engaged in meaning-focused communication, and their attention is briefly drawn to the form before returning to the communicative task. This is more difficult for AI systems to implement because it requires the AI to maintain a communicative interaction, identify moments when the learner's production deviates from the target in ways that would benefit from attention to form, and intervene briefly and non-disruptively before returning to the communicative flow.

LLM-based conversation systems have the potential to implement focus on form in ways that traditional CALL systems cannot. An LLM conversation partner that is engaged in a genuine exchange of meaning with the learner could, in principle, notice a grammatical error, provide a brief recast or metalinguistic hint, and then continue the conversation -- the kind of incidental, reactive focus on form that Long (1991) advocated. The technical capability exists; the challenge is designing the system to implement this strategy reliably and appropriately.

---

## 9.7 The Implicit/Explicit Knowledge Interface and AI

### 9.7.1 Defining Implicit and Explicit Knowledge

R. Ellis (2004, 2009) distinguished between implicit and explicit grammatical knowledge along several dimensions. Implicit knowledge is unconscious, intuition-based, accessible through automatic processing, and deployed in fluent real-time communication. Explicit knowledge is conscious, rule-based, accessible through controlled processing, and deployed when the learner has time to monitor their output.

Both types of knowledge contribute to L2 performance, but they contribute differently. In spontaneous conversation, implicit knowledge predominates because there is insufficient time for conscious rule application. In careful writing with opportunity for revision, explicit knowledge can supplement implicit knowledge through monitoring. In grammar tests, the type of knowledge measured depends on the test format: timed grammaticality judgments tap implicit knowledge, while untimed rule-stating tasks tap explicit knowledge.

### 9.7.2 AI and the Implicit Knowledge Problem

AI grammar instruction faces a fundamental challenge: the dimension of grammatical knowledge that AI can most easily develop (explicit knowledge) is not the dimension that most directly supports fluent communicative use (implicit knowledge). When an AI system teaches a grammar rule, provides practice exercises, and evaluates learner performance, it is primarily developing explicit knowledge -- the conscious, verbalizable understanding of how the grammar works. Converting this explicit knowledge into the automatic, unconscious implicit knowledge that drives fluent production is a separate process that requires extensive meaningful practice in communicative contexts.

This is DeKeyser's proceduralization challenge, discussed in Section 9.3, and it represents the single greatest limitation of AI grammar instruction as currently designed. Most AI grammar tools operate entirely in the explicit knowledge domain: they present rules, test rule application, and provide rule-based feedback. The step from "knowing the rule" to "using the structure automatically in communication" is largely left to the learner.

Some AI systems have begun to address this gap. Duolingo's progression from controlled exercises to more open-ended production tasks represents an attempt to move learners from explicit to proceduralizing knowledge. LLM-based conversation practice, where the learner must produce grammatical structures in real-time communicative interaction, creates conditions for proceduralization that rule-presentation exercises cannot. Adaptive systems that gradually increase time pressure -- giving learners less time to respond as they demonstrate mastery -- can push learners from controlled to automatic processing.

### 9.7.3 Implicit Grammar Learning Through AI Input

An alternative pathway to implicit grammatical knowledge, supported by usage-based theories (Ellis, 2002) and input-based theories (VanPatten, 2004), bypasses explicit instruction entirely. On this view, learners acquire grammar implicitly through exposure to large quantities of meaning-bearing input that contains the target structures in sufficiently frequent and salient contexts.

AI can support implicit grammar learning by providing massive quantities of comprehensible input -- adapted readings, listening materials, and conversational interaction -- that is structured to contain frequent, salient examples of target structures. This "input flood" approach (Trahey & White, 1993) does not teach grammar explicitly but ensures that the learner encounters the target form frequently enough for the implicit learning mechanisms to extract the relevant pattern.

The advantage of AI-mediated input flood is scalability and personalization: the AI can generate or select input texts that contain high concentrations of a target structure while remaining meaningful and engaging. The disadvantage is that input flood alone, without attention-drawing intervention, may not be sufficient for acquiring structures that are not perceptually salient or that conflict with L1 transfer (White, 1991). For such structures, some form of input enhancement or explicit instruction may be necessary to supplement the implicit exposure.

---

## 9.8 VanPatten's Processing Instruction and AI Applications

### 9.8.1 Input Processing Theory

VanPatten's (1996, 2004, 2015) Input Processing (IP) theory examines how learners derive intake from input -- specifically, how they assign grammatical roles and form-meaning connections during real-time comprehension. IP theory identifies several processing strategies that learners use by default, some of which lead to incorrect or incomplete grammatical processing:

**The First Noun Principle**: Learners tend to assign the first noun (or pronoun) in a sentence the role of agent/subject. This strategy works for canonical SVO sentences ("The dog chased the cat") but leads to misinterpretation of non-canonical structures like passives ("The cat was chased by the dog" -- interpreted as the cat doing the chasing) and OSV constructions.

**The Lexical Preference Principle**: When both a lexical item (e.g., *yesterday*) and a grammatical form (e.g., past tense -ed) encode the same meaning (past time), learners tend to process the lexical item and ignore the grammatical form. This means that in sentences like "Yesterday I walked to school," the learner processes *yesterday* as the indicator of past time and may not attend to the -ed suffix -- undermining acquisition of the morphological form.

**The Sentence Location Principle**: Learners tend to process items in sentence-initial and sentence-final positions more readily than items in medial positions. Grammatical morphemes that occur in medial positions (e.g., auxiliary verbs, inflectional morphology) receive less processing attention.

### 9.8.2 Processing Instruction

Processing Instruction (PI), the pedagogical application of IP theory, is designed to push learners away from their default, inefficient processing strategies toward more target-like processing. PI consists of three components:

1. **Explicit information**: The learner receives a brief explanation of the target grammatical structure and the processing strategy that they may be incorrectly applying.

2. **Structured input activities**: The learner engages in comprehension activities that are designed to make the default processing strategy fail. For example, to counter the First Noun Principle, a structured input activity might present sentences where the first noun is not the agent ("The boy was pushed by the girl") and ask the learner to identify who did the pushing. Because the default strategy produces the wrong answer, the learner is forced to process the grammatical form (passive voice) rather than relying on the positional heuristic.

3. **No production required**: Critically, PI does not require the learner to produce the target structure -- only to comprehend it. The theory predicts that changed processing of input will lead to both improved comprehension and improved production, because the restructured intake feeds both receptive and productive systems.

The empirical support for PI is substantial. VanPatten and Cadierno (1993) demonstrated that PI was as effective as traditional production-based instruction for improving production accuracy and more effective for improving interpretation accuracy. Subsequent studies (Benati, 2005; VanPatten & Wong, 2004; Marsden, 2006) have replicated and extended these findings across different structures and languages, establishing PI as one of the most empirically validated grammar instruction approaches in SLA.

### 9.8.3 AI as a Vehicle for Processing Instruction

Processing Instruction is exceptionally well-suited to AI implementation for several reasons:

**The structured input activities are highly systematizable**. Each activity presents a sentence, asks the learner a comprehension question, and provides feedback on whether the learner's interpretation was correct. This is precisely the kind of structured, interactive, feedback-rich activity that adaptive AI systems excel at delivering.

**The activities require no production**, only comprehension. This eliminates the need for AI to parse and evaluate learner-generated language -- a task where AI systems are less reliable -- and instead requires only presentation of stimuli and evaluation of multiple-choice or binary responses.

**The activities can be generated algorithmically**. For a given target structure and processing strategy, an AI can generate a large number of structured input items that vary the content while maintaining the structural properties necessary to push the learner toward target-like processing. An LLM can produce hundreds of sentences where the first noun is not the agent (for First Noun Principle activities), varying the vocabulary, context, and content to maintain engagement.

**PI requires individualized pacing but not individualized content**. The structured input activities are the same for all learners targeting the same structure; what varies is how many activities the learner needs before their processing changes. AI can adapt the volume of practice to the individual learner's performance, advancing them to the next structure when their processing demonstrates consistent change.

Despite these advantages, PI has been implemented in very few AI grammar tools. The reasons are partly practical (PI is less well-known among educational technology developers than traditional grammar instruction approaches) and partly commercial (comprehension-based activities are perceived as less engaging than production-based activities by many learners and app store reviewers). This represents a significant missed opportunity: PI is one of the most effective and well-researched grammar instruction approaches in SLA, and AI is an ideal delivery mechanism for it.

### 9.8.4 Designing AI-PI Systems

A well-designed AI system implementing Processing Instruction would operate as follows:

1. **Diagnostic phase**: The system identifies the learner's current processing strategies through comprehension tasks. For example, presenting passive sentences and asking "Who did the action?" reveals whether the learner is applying the First Noun Principle.

2. **Explicit information phase**: The system provides a brief, clear explanation of the target structure and the processing strategy the learner should avoid, using the learner's L1 if available for contrastive explanation.

3. **Structured input phase**: The system presents a sequence of structured input activities, each requiring the learner to interpret a sentence in a way that forces attention to the grammatical form. Activities are presented in increasing complexity: referential activities (with clear right/wrong answers) precede affective activities (where the learner expresses a personal opinion about the content, requiring genuine comprehension).

4. **Adaptive progression**: The system tracks the learner's accuracy across structured input activities and advances to the next structure when performance indicates consistent target-like processing. If the learner struggles, the system provides additional practice items or returns to the explicit information phase with a different explanation.

5. **Transfer assessment**: Periodically, the system assesses whether improved comprehension has transferred to production, using spontaneous production tasks (e.g., picture description, narrative retelling) that elicit the target structure without explicitly cueing it.

---

## 9.9 Beyond Grammar Rules: Constructions, Patterns, and Usage-Based AI

### 9.9.1 The Construction Grammar Perspective

Construction Grammar (Goldberg, 1995, 2006) challenges the traditional rule-based view of grammar by proposing that grammatical knowledge consists not of abstract rules but of constructions -- form-meaning pairings at various levels of abstraction, from morphemes to complex syntactic patterns. On this view, the ditransitive construction (*She gave him a book*), the caused-motion construction (*She sneezed the napkin off the table*), and the resultative construction (*She hammered the metal flat*) are each stored as holistic form-meaning units, not derived from abstract rules.

The Construction Grammar perspective aligns more naturally with LLM architecture than traditional generative grammar does. LLMs learn constructions as statistical patterns -- exactly the kind of form-meaning associations that Construction Grammar describes. An LLM "knows" the ditransitive construction not as a rule (NP + V + NP + NP) but as a pattern of co-occurrence that encodes a particular meaning (transfer of an object from one entity to another).

This alignment suggests that LLM-based grammar instruction might be particularly effective at teaching constructions as holistic units rather than decomposing them into discrete rules. Instead of teaching "the indirect object comes before the direct object when..." an LLM-based system could expose learners to multiple instances of the ditransitive construction in meaningful contexts, allowing the implicit learning mechanisms to extract the pattern -- precisely the kind of usage-based learning that Ellis (2002) and Tomasello (2003) describe.

### 9.9.2 Data-Driven Learning and AI

Johns (1991) introduced Data-Driven Learning (DDL) -- the pedagogical use of corpus data to allow learners to discover grammatical patterns inductively. Instead of being told a rule, learners examine multiple authentic examples (concordance lines) and formulate their own generalizations about how a structure is used. DDL promotes the kind of deep, analytical processing that explicit rule presentation may not, and research has found positive effects for DDL on grammar learning (Boulton & Cobb, 2017).

AI can supercharge DDL by making corpus analysis accessible to learners who lack the technical skills to use concordance software. An LLM can function as a "conversational corpus" -- the learner asks "When do English speakers use 'would' versus 'used to'?" and the AI provides not a rule but a collection of authentic examples, patterns, and generalizations that the learner can examine and from which they can induce the relevant distinctions. This is DDL without the concordancer, and it has the potential to make inductive grammar learning accessible to a much broader learner population.

---

## 9.10 Research Evidence on AI Grammar Instruction

### 9.10.1 ICALL Effectiveness Studies

The research base on ICALL grammar instruction, while not as large as the broader CALL literature, consistently shows positive effects. Heift (2010) found that learners using the E-Tutor system for German grammar showed significant improvement on both controlled and freer production tasks. Nagata (2009) reported that Japanese learners using Robo-Sensei outperformed control groups on particle usage and verb conjugation. Amaral and Meurers (2011) found that TAGARELA users showed improved accuracy on Portuguese grammar tasks.

A common finding across these studies is that the adaptive, individualized feedback provided by ICALL systems produces better outcomes than the generic feedback provided by non-intelligent CALL materials. When the system can diagnose the specific nature of the learner's error and provide targeted feedback, learning outcomes improve. This finding supports the theoretical argument that grammar feedback should be individualized and error-specific rather than generic.

### 9.10.2 LLM-Based Grammar Instruction

Research on LLM-based grammar instruction is emerging rapidly. Kohnke, Moorhouse, and Zou (2023) found that Hong Kong university students who used ChatGPT for grammar study showed significant improvement on grammar tests and reported high satisfaction with the quality of AI explanations. However, the study also found that some students accepted incorrect AI explanations without questioning them, raising concerns about critical evaluation skills.

Han and Finkelstein (2024) compared grammar instruction from ChatGPT-4 to instruction from a human tutor and found no significant difference on grammar accuracy measures for intermediate-level learners. However, advanced learners performed significantly better with the human tutor, particularly on complex structures involving subtle meaning distinctions. This pattern suggests that AI grammar instruction may be adequate for well-defined, rule-governed structures but less effective for the nuanced, context-dependent grammatical choices that characterize advanced proficiency.

### 9.10.3 Adaptive Grammar Platforms

Studies of adaptive grammar platforms (Duolingo, Babbel, Busuu) have generally found positive effects on grammatical accuracy, particularly for beginning and intermediate learners. Loewen et al. (2019) found that Duolingo users showed measurable improvement on standardized grammar tests over an eight-week period. Vesselinov and Grego (2012) estimated that 34 hours of Duolingo instruction produced gains equivalent to a university semester of Spanish, though this finding has been contested on methodological grounds.

The limitation common to these studies is the reliance on controlled test measures (multiple choice, fill-in-the-blank) that may tap explicit rather than implicit knowledge. Whether AI-trained grammar knowledge transfers to spontaneous communicative use -- the critical test from an acquisition perspective -- remains underexplored.

---

## 9.11 Designing Principled AI Grammar Systems: A Synthesis

### 9.11.1 Integrating Theoretical Frameworks

Drawing on the theoretical analysis presented throughout this chapter, we can articulate an integrated framework for AI grammar instruction that incorporates insights from Processability Theory, Skill Acquisition Theory, Input Processing, and the implicit/explicit knowledge literature:

**Developmental sensitivity (from PT)**: AI grammar systems should assess the learner's developmental stage and prioritize structures that are within the learner's zone of processability. Structures beyond the next developmental stage should be deferred, regardless of their frequency in the input or their prominence in the curriculum.

**Declarative-to-procedural progression (from SAT)**: AI grammar instruction should follow the declarative-procedural-automatic sequence, beginning with explicit rule presentation, progressing through meaningful controlled practice, and culminating in communicative activities that require automatic processing of the target structure.

**Processing-focused activities (from PI)**: Comprehension-based structured input activities should precede production activities, particularly for structures where default processing strategies lead to incorrect interpretation. AI is an ideal vehicle for delivering the large quantities of structured input that PI requires.

**Focus on form in communication (from Long)**: AI grammar instruction should include communicative activities where attention to form is reactive and incidental, not pre-planned and decontextualized. LLM-based conversation that occasionally draws attention to grammatical accuracy within a meaning-focused exchange represents this approach.

**Both explicit and implicit pathways**: AI grammar systems should develop both explicit knowledge (through rule presentation and metalinguistic feedback) and implicit knowledge (through extensive input exposure, communicative practice, and automatization activities).

### 9.11.2 A Model Architecture

A principled AI grammar tutoring system would incorporate:

1. **Developmental diagnostic**: Assessment of the learner's processability stage using elicited production and comprehension tasks that reveal processing capacity, not just accuracy.

2. **Adaptive curriculum**: A grammar syllabus organized by developmental stage rather than traditional difficulty ordering, with structures sequenced according to processability predictions.

3. **Multi-phase instruction for each structure**:
   - Phase 1: Explicit information + structured input (PI approach)
   - Phase 2: Controlled meaningful practice with immediate feedback (SAT declarative stage)
   - Phase 3: Guided communicative activities with delayed feedback (SAT procedural stage)
   - Phase 4: Free communicative interaction with incidental focus on form (automatization)

4. **Dual assessment**: Regular assessment of both explicit knowledge (rule-based tasks) and implicit knowledge (timed, meaning-focused tasks) to track development on both dimensions.

5. **Input enhancement**: Integration of grammar instruction with reading and listening activities where target structures are enhanced (bolded, highlighted, frequency-boosted) to promote noticing within meaning-focused input processing.

---

## 9.12 Conclusion

Grammar instruction through AI occupies a paradoxical position. On one hand, AI systems can do things that no classroom teacher can: provide unlimited patient explanation, generate thousands of practice items, track individual error patterns with perfect recall, and deliver adaptive instruction at scale. On the other hand, the aspects of grammar learning that AI handles best -- explicit rule presentation and controlled practice -- are precisely the aspects that the SLA literature identifies as necessary but insufficient for genuine acquisition. The harder work of grammar learning -- developing implicit knowledge, proceduralizing rules through meaningful communication, acquiring structures in developmental sequence -- remains largely unaddressed by current AI tools.

The theoretical frameworks reviewed in this chapter -- Processability Theory, Skill Acquisition Theory, Input Processing, and the implicit/explicit knowledge interface -- converge on a set of principles that should guide AI grammar instruction but largely do not: grammar is acquired in a developmental sequence that constrains what can be taught when; explicit knowledge becomes implicit only through extensive meaningful practice; comprehension-based processing activities are a powerful and underutilized approach; and the goal of grammar instruction is not rule knowledge but the automatic, unconscious ability to use grammatical structures in real-time communication.

The tools exist to build AI grammar systems that honor these principles. LLMs can generate structured input activities. Adaptive algorithms can track developmental progress. Conversational AI can provide the communicative context for proceduralization. The missing ingredient is not technology but theoretical literacy among the people who design AI grammar tools. Too many current systems default to the grammar-translation paradigm -- present a rule, drill the rule, test the rule -- dressed up in adaptive algorithms and attractive interfaces but fundamentally unchanged from the pedagogical approach that the SLA field moved beyond decades ago.

The promise of AI grammar instruction will be realized only when the systems are designed not by engineers who know what is technically possible but by applied linguists who know what is pedagogically necessary -- or, better, by collaborations between both. The intelligent tutor must be intelligent not just computationally but theoretically, embodying the insights that decades of SLA research have produced about how grammar is learned, not just how it is described.

---

## References

Amaral, L., & Meurers, D. (2011). On using intelligent computer-assisted language learning in real-life foreign language teaching and learning. *ReCALL*, 23(1), 4-24.

Anderson, J. R. (1993). *Rules of the mind*. Lawrence Erlbaum Associates.

Benati, A. (2005). The effects of processing instruction, traditional instruction, and meaning-output instruction on the acquisition of the English past simple tense. *Language Teaching Research*, 9(1), 67-93.

Boulton, A., & Cobb, T. (2017). Corpus use in language learning: A meta-analysis. *Language Learning*, 67(2), 348-393.

Brown, R. (1973). *A first language: The early stages*. Harvard University Press.

Chomsky, N. (1965). *Aspects of the theory of syntax*. MIT Press.

DeKeyser, R. M. (2007). Skill acquisition theory. In B. VanPatten & J. Williams (Eds.), *Theories in second language acquisition* (pp. 97-113). Lawrence Erlbaum.

DeKeyser, R. M. (2015). Skill acquisition theory. In B. VanPatten & J. Williams (Eds.), *Theories in second language acquisition* (2nd ed., pp. 94-112). Routledge.

Dentella, V., Raffaelli, I., & Caglio, F. (2023). Systematic assessment of ChatGPT's grammatical knowledge. *Frontiers in Artificial Intelligence*, 6, 1232706.

Dulay, H. C., & Burt, M. K. (1974). Natural sequences in child second language acquisition. *Language Learning*, 24(1), 37-53.

Ellis, N. C. (2002). Frequency effects in language processing: A review with implications for theories of implicit and explicit language acquisition. *Studies in Second Language Acquisition*, 24(2), 143-188.

Ellis, R. (2004). The definition and measurement of L2 explicit knowledge. *Language Learning*, 54(2), 227-275.

Ellis, R. (2005). Measuring implicit and explicit knowledge of a second language: A psychometric study. *Studies in Second Language Acquisition*, 27(2), 141-172.

Ellis, R. (2006). Current issues in the teaching of grammar: An SLA perspective. *TESOL Quarterly*, 40(1), 83-107.

Ellis, R. (2009). Implicit and explicit learning, knowledge and instruction. In R. Ellis et al. (Eds.), *Implicit and explicit knowledge in second language learning, testing and teaching* (pp. 3-25). Multilingual Matters.

Erlam, R. (2005). Language aptitude and its relationship to instructional effectiveness in second language acquisition. *Language Teaching Research*, 9(2), 147-171.

Goldberg, A. E. (1995). *Constructions: A construction grammar approach to argument structure*. University of Chicago Press.

Goldberg, A. E. (2006). *Constructions at work: The nature of generalization in language*. Oxford University Press.

Goldschneider, J. M., & DeKeyser, R. M. (2001). Explaining the "natural order of L2 morpheme acquisition" in English: A meta-analysis of multiple determinants. *Language Learning*, 51(1), 1-50.

Gulordava, K., Baroni, M., & Boleda, G. (2018). Colorless green recurrent networks dream hierarchically. In *Proceedings of NAACL-HLT* (pp. 1195-1205).

Han, L., & Finkelstein, A. (2024). Comparing AI and human grammar tutors: Effects on accuracy and metalinguistic awareness. *Language Learning & Technology*, 28(2), 1-22.

Heift, T. (2001). Intelligent language tutoring systems for grammar practice. *Zeitschrift fur Interkulturellen Fremdsprachenunterricht*, 6(2), 1-15.

Heift, T. (2010). Developing an intelligent language tutor. *CALICO Journal*, 27(3), 443-459.

Johns, T. (1991). Should you be persuaded: Two samples of data-driven learning materials. *ELR Journal*, 4, 1-16.

Keating, G. D., & Jegerski, J. (2015). Experimental designs in sentence processing research. *Studies in Second Language Acquisition*, 37(1), 1-32.

Kohnke, L., Moorhouse, B. L., & Zou, D. (2023). ChatGPT for language teaching and learning. *RELC Journal*, 54(2), 537-550.

Krashen, S. D. (1977). Some issues relating to the Monitor Model. In H. D. Brown, C. A. Yorio, & R. H. Crymes (Eds.), *On TESOL '77* (pp. 144-158). TESOL.

Krashen, S. D. (1981). *Second language acquisition and second language learning*. Pergamon.

Linzen, T., & Baroni, M. (2021). Syntactic structure from deep learning. *Annual Review of Linguistics*, 7, 195-212.

Loewen, S., Crowther, D., Isbell, D. R., Kim, K. M., Maloney, J., Miller, Z. F., & Raber, H. (2019). Mobile-assisted language learning: A Duolingo case study. *ReCALL*, 31(3), 293-311.

Long, M. H. (1991). Focus on form: A design feature in language teaching methodology. In K. de Bot, R. B. Ginsberg, & C. Kramsch (Eds.), *Foreign language research in cross-cultural perspective* (pp. 39-52). John Benjamins.

Marsden, E. (2006). Exploring input processing in the classroom: An experimental comparison of processing instruction and enriched input. *Language Learning*, 56(3), 507-566.

McCoy, R. T., Frank, R., & Linzen, T. (2020). Does syntax need to grow on trees? Sources of hierarchical inductive bias in sequence-to-sequence networks. *Transactions of the Association for Computational Linguistics*, 8, 125-140.

Nagata, N. (2009). Robo-Sensei's NLP-based error detection and feedback generation. *CALICO Journal*, 26(3), 562-579.

Nkambou, R., Bourdeau, J., & Mizoguchi, R. (Eds.). (2010). *Advances in intelligent tutoring systems*. Springer.

Norris, J. M., & Ortega, L. (2000). Effectiveness of L2 instruction: A research synthesis and quantitative meta-analysis. *Language Learning*, 50(3), 417-528.

Paradis, M. (2009). *Declarative and procedural determinants of second languages*. John Benjamins.

Pienemann, M. (1998). *Language processing and second language development: Processability theory*. John Benjamins.

Pienemann, M. (2005). *Cross-linguistic aspects of processability theory*. John Benjamins.

Spada, N., & Tomita, Y. (2010). Interactions between type of instruction and type of language feature: A meta-analysis. *Language Learning*, 60(2), 263-308.

Tomasello, M. (2003). *Constructing a language: A usage-based theory of language acquisition*. Harvard University Press.

Trahey, M., & White, L. (1993). Positive evidence and preemption in the second language classroom. *Studies in Second Language Acquisition*, 15(2), 181-204.

VanPatten, B. (1996). *Input processing and grammar instruction in second language acquisition*. Ablex.

VanPatten, B. (2004). *Processing instruction: Theory, research, and commentary*. Lawrence Erlbaum.

VanPatten, B. (2015). Input processing in adult SLA. In B. VanPatten & J. Williams (Eds.), *Theories in second language acquisition* (2nd ed., pp. 113-134). Routledge.

VanPatten, B., & Cadierno, T. (1993). Explicit instruction and input processing. *Studies in Second Language Acquisition*, 15(2), 225-243.

VanPatten, B., & Wong, W. (2004). Processing instruction and the French causative: Another replication. In B. VanPatten (Ed.), *Processing instruction: Theory, research, and commentary* (pp. 97-118). Lawrence Erlbaum.

Vesselinov, R., & Grego, J. (2012). *Duolingo effectiveness study*. City University of New York.

White, L. (1991). Adverb placement in second language acquisition: Some effects of positive and negative evidence in the classroom. *Second Language Research*, 7(2), 133-161.

Wilcox, E. G., Levy, R., Morita, T., & Futrell, R. (2018). What do RNN language models learn about filler-gap dependencies? In *Proceedings of the EMNLP Workshop on Analyzing and Interpreting Neural Networks for NLP* (pp. 211-221).
