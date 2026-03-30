# Chapter 11: Assessment, Testing, and AI

## Introduction: The Pivot Point Where Assessment and Learning Merge

Assessment has always occupied a paradoxical position in language education. It is simultaneously the most consequential and the most contested dimension of pedagogical practice. High-stakes language tests determine who gains admission to universities, who receives professional certifications, who obtains visas and citizenship, and who is placed in advanced or remedial courses. The stakes are real, the consequences life-altering, and the trust placed in assessment instruments is correspondingly immense. Yet the history of language testing is also a history of critique: concerns about construct validity, cultural bias, washback effects, and the reduction of complex communicative competence to numerical scores have animated applied linguistics scholarship for decades (Bachman & Palmer, 2010; McNamara, 2000; Shohamy, 2001).

Into this already contested terrain, artificial intelligence has arrived with a dual promise. On one hand, AI offers unprecedented efficiency: automated essay scoring systems can evaluate thousands of writing samples in minutes, computer-adaptive testing algorithms can identify a learner's proficiency level with fewer items than traditional fixed-form tests, and learning analytics can transform every interaction into a data point for continuous, embedded assessment. On the other hand, AI introduces new risks at a scale that the field has not previously confronted: algorithmic bias that may systematically disadvantage certain populations, construct underrepresentation when AI systems assess only what they can quantify, the erosion of human judgment in high-stakes decisions, and the normalization of surveillance-based assessment paradigms that treat every learner action as evidence to be harvested.

This chapter argues that AI-powered assessment represents not merely a technological upgrade to existing testing practices but a fundamental reconceptualization of the relationship between assessment and learning. When assessment becomes continuous, embedded, and invisible--when the AI system is always assessing, always adapting, always generating data--the traditional distinction between instruction and assessment dissolves. This dissolution has transformative potential: dynamic assessment, formative feedback loops, and personalized learning trajectories that were theoretically desirable but practically impossible become achievable. But it also carries profound risks: the gamification of learning, the reduction of complex competence to algorithmically tractable features, and the displacement of professional teacher judgment by opaque computational processes.

The chapter begins with the theoretical foundations of language assessment, establishing the constructs and standards against which AI systems must be evaluated. It then examines specific AI assessment technologies--automated essay scoring, automated speech assessment, computer-adaptive testing, and learning analytics--with attention to both their capabilities and their documented limitations. It turns to the critical issues of bias, fairness, and construct validity that AI assessment amplifies. Finally, it explores the concept of dynamic assessment and the promise of assessment-learning integration that AI makes possible, while insisting that this promise be pursued within a framework of ethical accountability.

---

## 11.1 Theoretical Foundations of Language Assessment

### 11.1.1 Construct Validity: What Are We Measuring?

The concept of construct validity, as elaborated by Messick (1989) and applied to language assessment by Bachman and Palmer (1996, 2010), provides the foundational framework for evaluating any assessment instrument, including AI-powered ones. Construct validity asks a deceptively simple question: Does the assessment measure what it claims to measure? In language assessment, the "construct" is typically some aspect of communicative language ability--reading comprehension, writing proficiency, speaking fluency, grammatical competence--and the validity argument must demonstrate that the scores produced by the assessment reflect that construct rather than irrelevant factors.

Messick's (1989) unified theory of validity encompasses several facets that are directly relevant to AI assessment. Content validity asks whether the assessment tasks adequately represent the construct domain. Structural validity asks whether the internal structure of the assessment (the relationships among items, components, and scores) is consistent with the theoretical structure of the construct. External validity asks whether scores relate to other measures in theoretically predicted ways. Consequential validity--Messick's most controversial contribution--asks whether the social consequences of assessment use are justifiable and whether the assessment contributes to, or undermines, the values it claims to serve.

For AI-powered assessment, each of these validity facets raises distinctive concerns. Content validity is threatened when AI assessment operationalizes only those aspects of communicative competence that are computationally tractable, potentially excluding pragmatic appropriateness, sociolinguistic variation, intercultural competence, and other dimensions that resist algorithmic evaluation. Structural validity is challenged when AI scoring algorithms treat language proficiency as a composite of separately measurable subskills rather than as an integrated, context-dependent capacity. Consequential validity is at stake when AI assessment systems, deployed at scale with apparent objectivity, reinforce existing inequities or narrow curricula in ways that harm the learners they claim to serve.

### 11.1.2 Bachman and Palmer's Assessment Framework

Bachman and Palmer's (2010) framework for language assessment use provides the most comprehensive set of principles for evaluating language tests, and it is directly applicable to AI-powered assessment. The framework identifies six qualities of assessment usefulness: reliability, construct validity, authenticity, interactiveness, impact, and practicality. These qualities exist in tension--maximizing one may compromise another--and the design of any assessment represents a set of tradeoffs among them.

AI assessment technologies shift the tradeoff landscape in specific ways. Practicality and reliability are dramatically enhanced: AI scoring eliminates rater fatigue, produces perfectly consistent scores across thousands of responses, and reduces the cost and time of assessment delivery. However, these gains in practicality and reliability may come at the cost of construct validity (if AI scoring captures only surface-level features of language proficiency), authenticity (if tasks must be constrained to formats that AI can score), and interactiveness (if the assessment experience is reduced to human-machine interaction devoid of genuine communicative purpose).

Impact--particularly washback--deserves special attention. Washback refers to the influence of a test on teaching and learning, and it is well-established that high-stakes tests shape curriculum, instruction, and learner behavior (Alderson & Wall, 1993; Cheng, 2005). When an AI scoring system rewards certain textual features (lexical diversity, syntactic complexity, discourse coherence markers) and ignores others (rhetorical effectiveness, audience awareness, cultural sensitivity), teachers and learners will orient their efforts toward the rewarded features. The washback effects of AI assessment may be particularly powerful because the scoring criteria are often opaque--learners and teachers cannot inspect the algorithm as they might inspect a rubric--creating a black-box effect that generates anxiety and strategic test-taking behavior without the transparency needed for productive learning.

### 11.1.3 Dynamic Assessment: Vygotsky, Lantolf, and the Zone of Proximal Development

Dynamic assessment (DA), grounded in Vygotsky's (1978) Sociocultural Theory and elaborated for L2 contexts by Lantolf and Poehner (2004, 2011), represents a theoretical alternative to the static assessment paradigm that dominates current practice. In static assessment, the assessor presents tasks, records the learner's unassisted performance, and uses that performance as the basis for scoring and placement. The learner's score reflects their independent performance level--what Vygotsky called the "actual developmental level."

Dynamic assessment, by contrast, integrates assessment and instruction: the assessor provides graduated mediation (hints, prompts, leading questions, explicit instruction) during the assessment process, and the learner's responsiveness to that mediation becomes a key datum. DA assesses not only what the learner can do independently but what they can do with assistance--their Zone of Proximal Development (ZPD). The argument is that ZPD-based assessment provides a richer, more predictive picture of learner ability than static assessment because it reveals developmental potential, not just current achievement.

AI technologies make large-scale dynamic assessment feasible for the first time. In a traditional DA session, a trained assessor must interact one-on-one with each learner, providing individualized mediation and interpreting the learner's responses in real time--a process that is rich but logistically prohibitive for most educational contexts. An AI-powered DA system could provide graduated mediation algorithmically, tracking which levels of support the learner requires and using that information to estimate ZPD boundaries. The system could adapt in real time: if a learner fails an item, the AI provides increasingly explicit support until the learner succeeds, and the level of support required becomes part of the score.

Lantolf and Poehner (2014) have explored computerized dynamic assessment (C-DA) prototypes that implement this approach, and the results are promising: C-DA systems produce scores that correlate with but are not identical to static test scores, and the mediation-responsiveness data provides additional predictive validity for future learning. However, current C-DA implementations are limited to relatively constrained task types (vocabulary, grammar, reading comprehension) where graduated mediation can be pre-scripted. The extension of dynamic assessment to more complex, open-ended language tasks--writing, speaking, pragmatic interaction--awaits the development of AI systems capable of providing contextualized, responsive mediation in real time. LLM-powered tutoring systems may approach this capability, but the leap from pre-scripted hint sequences to genuine Vygotskian mediation is substantial and not yet achieved.

---

## 11.2 Automated Essay Scoring: The Most Controversial AI Assessment Technology

### 11.2.1 A Brief History of AES

Automated essay scoring (AES) is the oldest and most extensively researched application of AI to language assessment. The first AES system, Ellis Page's Project Essay Grade (PEG), dates to 1966 and used surface-level text features (word length, sentence length, punctuation counts) as proxies for writing quality. Despite its simplicity, PEG achieved moderate correlations with human rater scores, establishing the surprising finding that surface features of text are statistically associated with human judgments of quality--a finding that has sustained the AES enterprise for six decades while simultaneously constituting its most fundamental vulnerability.

The evolution of AES mirrors the broader trajectory of NLP. Feature-based systems like PEG gave way to more sophisticated approaches: the Educational Testing Service's e-rater (Attali & Burstein, 2006) uses over 100 linguistic features organized into categories (grammar, usage, mechanics, style, organization, development); Pearson's Intelligent Essay Assessor (Landauer, Laham, & Foltz, 2003) applies Latent Semantic Analysis to evaluate content; Turnitin's Revision Assistant uses neural networks trained on scored essay corpora. Most recently, large language model-based approaches (fine-tuned versions of BERT, GPT, and similar architectures) have achieved the highest reported agreement rates with human raters (Wang, Shang, Liou, Shih, & Chen, 2023).

### 11.2.2 The Agreement Illusion

The standard metric for evaluating AES systems is agreement with human raters, typically measured by quadratic weighted kappa or exact/adjacent agreement percentages. Proponents of AES regularly cite agreement rates between AI scores and human scores that equal or exceed agreement rates between two human raters. ETS reports that e-rater achieves adjacent agreement with human raters of approximately 92-97% across TOEFL iBT and GRE essay prompts (Attali & Burstein, 2006). These figures are impressive and are routinely invoked to argue that AI scoring is "as good as" human scoring.

This argument, however, contains a fundamental logical flaw that has been identified by numerous assessment scholars (Deane, 2013; Perelman, 2014; Ericsson & Haswell, 2006). Agreement with human raters does not demonstrate that the AI system measures the same construct as human raters. Two instruments can produce similar scores for entirely different reasons. A thermometer and a barometer might both produce higher readings on sunny days, but they are measuring different things. Similarly, an AES system that assigns high scores to essays with varied vocabulary, long sentences, and frequent discourse markers may agree with human raters who assign high scores for clear argumentation, effective evidence use, and audience awareness--because these features tend to co-occur in proficient writing--without actually measuring argumentation, evidence use, or audience awareness at all.

The "agreement illusion" has been demonstrated empirically by researchers who have generated texts specifically designed to exploit AES scoring features. Perelman (2014) famously generated gibberish essays that received high e-rater scores by using sophisticated vocabulary, complex syntax, and formulaic discourse markers while saying nothing meaningful. His "BABEL generator" produced texts that were lexically and syntactically complex but semantically vacuous, earning scores comparable to proficient human writing. More recently, Yan and Chung (2023) demonstrated that LLM-generated essays--which excel at surface coherence while potentially lacking genuine critical thinking--receive systematically higher AES scores than equivalent human-written essays, raising concerns about what AES systems are actually rewarding.

### 11.2.3 What AES Actually Measures

The question of what AES systems actually measure--as opposed to what they claim to measure--is a construct validity question of the first order. A substantial body of research suggests that AES systems are most sensitive to:

**Lexical features**: vocabulary diversity (type-token ratio, lexical sophistication), word frequency profiles, and academic word use. These features are moderately correlated with writing proficiency but can be inflated by thesaurus use, formulaic academic language, or LLM-generated text.

**Syntactic complexity**: sentence length, clause density, subordination ratio, and syntactic variety. These features correlate with developmental level but do not distinguish between purposeful complexity (used effectively for communicative goals) and gratuitous complexity (used to appear sophisticated).

**Mechanical accuracy**: spelling, punctuation, subject-verb agreement, and other surface-level error types. These are the most reliably measured features but also the least interesting from a communicative competence perspective.

**Discourse markers and organization**: the presence of explicit cohesive devices (however, furthermore, in conclusion), paragraph structure, and transition patterns. These features indicate awareness of academic writing conventions but may reward formulaic organization over genuine rhetorical effectiveness.

What AES systems measure poorly or not at all includes: the quality and relevance of argumentation, the accuracy and appropriateness of evidence, cultural sensitivity and audience awareness, voice and rhetorical stance, originality and creativity, and the pragmatic appropriateness of register and style for a given communicative context. These are not marginal aspects of writing proficiency; they constitute the core of what expert readers evaluate when they assess writing quality. Their absence from AES evaluation represents a significant construct underrepresentation.

### 11.2.4 AES in L2 Writing Assessment

For second language writers, the limitations of AES are compounded by several additional concerns. L2 writers may produce texts that are linguistically simple but communicatively effective--using high-frequency vocabulary and short, clear sentences to convey meaning successfully. An AES system that rewards lexical sophistication and syntactic complexity may systematically undervalue such writing, penalizing communicative success in favor of surface-level complexity.

Conversely, L2 writers may produce texts with numerous surface-level errors that nonetheless demonstrate sophisticated rhetorical strategies, cultural knowledge, and critical thinking. A human rater can see past the errors to evaluate the underlying competence; an AES system that weights mechanical accuracy heavily cannot. This differential sensitivity has equity implications: L2 writers from educational backgrounds that emphasized communicative competence over formal accuracy may be systematically disadvantaged by AES systems, even when their communicative writing ability is strong.

Weigle (2013) has documented additional concerns specific to L2 AES assessment, including the potential for L1-specific error patterns to interact unpredictably with AES scoring models trained primarily on L1 English writing, the question of whether AES scoring rubrics developed for L1 writers are appropriate for L2 assessment, and the risk that AES-driven washback may orient L2 writing instruction toward surface-level accuracy at the expense of communicative development.

---

## 11.3 Automated Speech Assessment

### 11.3.1 The Architecture of Automated Speaking Tests

Automated speech assessment systems extend the AI assessment paradigm from writing to speaking. The most widely used commercial systems include Pearson's Versant (used for placement and certification), ETS's SpeakWrite (a component of the TOEFL iBT practice system), and Duolingo's English Test speaking section. These systems combine ASR technology (discussed in Chapter 10) with additional NLP components for evaluating content, fluency, vocabulary, and grammar.

The typical architecture of an automated speaking test involves several processing stages: the ASR engine transcribes the learner's speech into text; acoustic feature extractors measure duration, pitch, energy, and spectral characteristics; the transcript is analyzed for grammatical accuracy, lexical diversity, and content relevance; fluency metrics (speech rate, pause frequency, pause duration, repetition rate) are computed from the acoustic signal; and a machine learning model combines these features into a holistic proficiency score, typically calibrated against human rater scores from a training corpus.

### 11.3.2 What Automated Speaking Tests Can and Cannot Measure

Automated speaking tests have demonstrated reasonable validity for measuring certain aspects of speaking proficiency. Fluency features (speech rate, pause patterns, mean length of run) are particularly well-captured by automated systems, and these features are among the strongest predictors of human ratings of speaking proficiency (Ginther, Dimova, & Yang, 2010). Pronunciation accuracy at the segmental level can be assessed with moderate reliability (see Chapter 10). Grammatical accuracy and lexical diversity in transcribed speech can be evaluated using the same NLP techniques applied to writing.

However, automated speaking tests face several limitations that are more severe than those affecting AES. First, ASR transcription errors propagate through the entire scoring pipeline: if the ASR system misrecognizes a word, the downstream grammar, vocabulary, and content analyses are based on erroneous input. Transcription errors are not random; they are systematically more frequent for speakers with certain L1 backgrounds, accents, and speech patterns (see Chapter 10), meaning that scoring errors are inequitably distributed across populations.

Second, automated speaking tests struggle with the interactional and pragmatic dimensions of speaking proficiency. The ability to manage turn-taking, repair misunderstandings, adapt register to context, use humor or irony appropriately, and negotiate meaning with an interlocutor--all core aspects of communicative speaking competence--cannot be assessed in the monologic response formats that automated systems require. The task types amenable to automated scoring (read-aloud passages, picture descriptions, opinion statements with preparation time) are the least communicatively authentic, and they may systematically underrepresent the construct of speaking proficiency as defined by contemporary communicative frameworks (Bachman & Palmer, 2010; Council of Europe, 2001).

Third, the suprasegmental and discourse-level features that most strongly influence human judgments of speaking proficiency--prosodic appropriateness, discourse coherence, pragmatic force--are the features most difficult for automated systems to evaluate (Xi, 2010). This creates a construct validity gap: automated speaking scores reflect fluency and accuracy more strongly than communicative effectiveness, potentially rewarding rapid, grammatically accurate but communicatively flat speech over slower, less accurate but pragmatically skilled performance.

### 11.3.3 The Duolingo English Test: A Case Study

The Duolingo English Test (DET) merits specific examination as the most prominent AI-native language assessment currently in wide use. Unlike the TOEFL iBT or IELTS, which were designed as human-scored assessments with AI components added later, the DET was designed from the ground up as a computer-adaptive, partially AI-scored test. It uses a combination of item types: some are fully computer-scored (C-test items, dictation, read-aloud), while others (speaking and writing samples) use AI scoring with human score verification.

The DET's validity argument (LaFlair & Egbert, 2022) is built on several pillars: strong correlations with established tests (TOEFL, IELTS), internal factor structure consistent with a general language proficiency construct, and increasing acceptance by universities worldwide (over 5,000 institutions as of 2025). However, the test has also attracted criticism on several grounds: the adaptive algorithm's item selection process is proprietary and not available for independent validation; the speaking and writing tasks are constrained to formats amenable to AI scoring, potentially underrepresenting communicative competence; and the test's 45-minute administration time, while convenient, raises questions about whether such a brief assessment can adequately sample the construct domain.

The DET represents a harbinger of a broader trend: assessments designed around AI scoring capabilities rather than AI scoring adapted to existing assessment designs. This approach has the advantage of internal coherence--the tasks and the scoring are mutually optimized--but the risk of construct definition being driven by technological feasibility rather than theoretical adequacy. If the construct of "English proficiency" is operationally defined as "whatever can be reliably scored by an AI system in 45 minutes," the construct may shrink to fit the technology rather than the technology expanding to capture the construct.

---

## 11.4 Computer-Adaptive Testing and AI-Powered Placement

### 11.4.1 Item Response Theory and CAT

Computer-adaptive testing (CAT) represents one of the most theoretically grounded applications of AI to language assessment. CAT is built on Item Response Theory (IRT), a psychometric framework that models the probability of a correct response as a function of the learner's ability level and the item's characteristics (difficulty, discrimination, guessing parameter). In a CAT system, the algorithm selects each subsequent item based on the learner's responses to previous items, targeting items near the estimated ability boundary to maximize measurement precision.

The result is a test that is both shorter and more precise than a fixed-form test: a well-designed CAT can estimate a learner's ability level with the same precision as a conventional test using 50-70% fewer items (Wainer et al., 2000). For language placement--where large numbers of learners must be assessed quickly and accurately--CAT offers an compelling value proposition. Several major language placement systems now use CAT or adaptive algorithms, including the Oxford Placement Test, the DIALANG diagnostic assessment, and proprietary placement systems used by universities and language programs.

### 11.4.2 AI-Enhanced Adaptive Algorithms

Recent advances extend traditional CAT beyond IRT-based item selection to incorporate machine learning and deep learning algorithms. These "AI-enhanced" adaptive systems can model learner ability along multiple dimensions simultaneously (multidimensional CAT), account for temporal patterns in learner performance (detecting fatigue, warm-up effects, or test-taking strategies), and incorporate non-response data (time spent on items, answer changes, navigation patterns) into ability estimation.

Bayesian knowledge tracing (BKT) and deep knowledge tracing (DKT) represent the most sophisticated approaches to adaptive assessment. BKT models learner knowledge as a binary latent variable (known/unknown) for each knowledge component, updating the probability estimate with each response. DKT uses recurrent neural networks to model learner knowledge as a continuous vector, capturing complex dependencies among knowledge components and temporal patterns that BKT cannot. Both approaches promise more nuanced ability estimation than traditional IRT, but they also raise concerns about model interpretability: while an IRT model produces transparent item parameters and ability estimates, a deep learning model's internal representations are opaque, making it difficult to explain to stakeholders why a learner received a particular score or placement.

### 11.4.3 The Diagnostic Potential of Adaptive Assessment

One of the most promising applications of AI-powered adaptive assessment is diagnostic assessment--identifying not just a learner's overall proficiency level but their specific strengths and weaknesses across linguistic subdomains. Traditional proficiency tests produce a single score or a small number of subscores; a diagnostic AI assessment could produce a detailed learner profile specifying relative competence in grammar, vocabulary (by frequency band and domain), reading (by text type and processing level), listening (by speech rate and accent), and speaking (by fluency, accuracy, and complexity).

Such profiles could inform individualized learning plans, guiding learners and teachers to focus on areas of greatest need. The adaptive algorithm could also be used for ongoing diagnostic monitoring, reassessing the learner's profile periodically and adjusting instructional recommendations as the profile changes. This application moves adaptive testing from a one-time placement event to a continuous assessment-instruction loop--the kind of integration that dynamic assessment theory envisions but that static testing cannot deliver.

The technical feasibility of fine-grained diagnostic assessment depends on the availability of test items that isolate specific knowledge components and the accuracy of the inference model that maps response patterns to diagnostic profiles. For well-studied domains like English grammar and vocabulary, the item banks and inference models are mature. For less well-studied domains (pragmatic competence, sociolinguistic variation, discourse structure) and for less commonly tested languages, the infrastructure does not yet exist.

---

## 11.5 Formative Assessment and Learning Analytics

### 11.5.1 The Promise of Continuous, Embedded Assessment

The most transformative potential of AI in language assessment lies not in the improvement of summative testing but in the integration of assessment into the fabric of everyday learning. Formative assessment--assessment for learning rather than assessment of learning (Black & Wiliam, 1998)--has been shown to produce substantial learning gains when implemented effectively: Hattie's (2009) synthesis of meta-analyses identifies formative assessment as one of the most powerful pedagogical interventions available, with effect sizes exceeding d = 0.70.

However, effective formative assessment is labor-intensive. It requires teachers to continuously monitor learner performance, identify patterns of difficulty, provide timely and specific feedback, and adjust instruction accordingly. In language classrooms with 20-30 students producing written and spoken output continuously, this monitoring-feedback cycle exceeds what any human teacher can sustain. AI can, in principle, fill this gap: analyzing learner output in real time, identifying recurring error patterns, providing immediate corrective feedback, and generating data that teachers can use for instructional planning.

The vision of continuous, embedded assessment aligns with the SLA processing pipeline framework established in earlier chapters. If assessment occurs naturally within input-interaction-output-feedback cycles, it ceases to be a separate, anxiety-inducing event and becomes an integral part of the learning process. The learner practices speaking with an AI tutor (Chapter 5), the AI system evaluates pronunciation, fluency, grammar, and vocabulary in real time (Chapters 7, 10, this chapter), provides corrective feedback (Chapter 7), and adjusts subsequent input difficulty accordingly (Chapter 4). Assessment, instruction, and feedback merge into a single adaptive loop.

### 11.5.2 Learning Analytics: Data, Dashboards, and Decisions

Learning analytics--the collection, analysis, and reporting of data about learner behavior and performance--provides the infrastructure for continuous assessment. In AI-powered language learning platforms, learning analytics can track a vast array of data points: time on task, response accuracy, response latency, error patterns, vocabulary growth trajectories, fluency development curves, content engagement patterns, and learner self-assessment data.

The utility of learning analytics depends on what is done with the data. Three levels of analytics are typically distinguished (Siemens, 2013):

**Descriptive analytics** summarize what has happened: how many hours the learner has practiced, which skills they have worked on, how their accuracy has changed over time. Descriptive analytics are the most common and least controversial application; they provide useful summaries for learners and teachers but do not, by themselves, drive instructional decisions.

**Predictive analytics** use historical data to forecast future outcomes: which learners are at risk of not meeting proficiency targets, which learners are likely to benefit from additional pronunciation practice, which learners' vocabulary growth has plateaued. Predictive analytics have significant potential for early intervention but also raise concerns about self-fulfilling prophecy effects: if a system predicts that a learner will struggle, and resources are withdrawn or the learner is tracked into a lower group, the prediction may be confirmed by the intervention it triggers rather than by the learner's inherent ability.

**Prescriptive analytics** go furthest, recommending specific actions: "This learner should review past tense irregular forms," "This learner would benefit from extensive reading at the 3,000-word frequency level," "This learner's speaking fluency has stagnated and conversational practice should be increased." Prescriptive analytics embed pedagogical judgments in algorithmic recommendations, and the quality of those judgments depends on the quality of the pedagogical model underlying the algorithm--a model that is rarely made explicit and even more rarely subjected to independent validation.

### 11.5.3 The Teacher's Role in AI-Mediated Assessment

The integration of AI into formative assessment does not eliminate the need for teacher judgment; if anything, it increases it. Teachers must decide which AI-generated data to attend to and which to ignore, how to interpret patterns that the AI system flags, whether to follow or override algorithmic recommendations, and how to communicate assessment information to learners in ways that support motivation and self-regulation rather than anxiety and dependence.

Rea-Dickins (2001) documented the complexity of teacher assessment practices in language classrooms, showing that experienced teachers draw on a wide range of cues--including paralinguistic, affective, and contextual information that no AI system currently captures--in forming their assessment judgments. The risk of AI-mediated formative assessment is not that it provides too little information but that it provides too much of the wrong kind: reams of quantitative data about surface-level linguistic features that crowd out the qualitative, contextual, and relational information that teachers need for effective formative assessment.

The optimal model is one in which AI handles the data-intensive monitoring that exceeds human capacity--tracking error patterns across dozens of students, identifying vocabulary gaps, flagging fluency stagnation--while the teacher retains authority over the interpretive, relational, and ethical dimensions of assessment. The AI system provides the data; the teacher provides the judgment. This division of labor requires that AI assessment data be presented to teachers in interpretable, actionable formats rather than as raw data dumps or opaque algorithmic recommendations.

---

## 11.6 Washback Effects of AI Assessment

### 11.6.1 Positive Washback Potential

AI assessment has the potential to generate positive washback--beneficial effects on teaching and learning--in several ways. Continuous formative assessment can promote a growth mindset by providing regular evidence of progress rather than periodic high-stakes judgments. Adaptive assessment can reduce test anxiety by matching item difficulty to learner ability, ensuring that learners are neither overwhelmed by items beyond their level nor bored by items below it. Diagnostic assessment can direct learner attention to specific areas of need, promoting more efficient and targeted study habits.

The immediacy of AI feedback may also enhance washback. Black and Wiliam (1998) identified timely feedback as a critical component of effective formative assessment, and AI systems can provide feedback within seconds of learner output--far faster than the days or weeks required for human-scored assessments. If this feedback is specific, actionable, and oriented toward improvement rather than judgment, it can support the kind of self-regulated learning that promotes long-term language development.

### 11.6.2 Negative Washback Risks

The negative washback potential of AI assessment is at least equally significant. When AI scoring criteria are opaque--as they typically are in commercial systems--learners and teachers may develop distorted mental models of what the system rewards, leading to strategic test-taking behavior that maximizes scores without improving genuine language ability. The "teach to the algorithm" phenomenon is already documented: studies of AES washback show that learners who understand that automated scoring rewards lexical sophistication and syntactic complexity may prioritize these features at the expense of content quality and argumentative coherence (Warschauer & Grimes, 2008).

The always-on nature of continuous AI assessment may also produce negative washback through surveillance effects. If every utterance, every writing sample, every interaction is being evaluated, learners may experience a panoptic anxiety (Foucault, 1977) that inhibits risk-taking, experimentation, and the productive struggle that SLA theory identifies as essential for acquisition. Swain's (1985) Output Hypothesis, for example, emphasizes that learners need to be "pushed" to produce output beyond their current comfort zone, which requires a willingness to make errors. An omnipresent assessment system that records and evaluates every error may discourage exactly this kind of productive risk-taking.

Furthermore, the gamification of AI-mediated assessment--progress bars, point systems, leaderboards, streak counters--may orient learner motivation toward extrinsic rewards rather than intrinsic engagement with the language. The extensive research on motivation in SLA (Dornyei, 2005; Ushioda, 2009) suggests that extrinsic motivation is a weaker and less sustainable driver of language acquisition than intrinsic motivation, and assessment systems that emphasize scores, rankings, and rewards may undermine the intrinsic motivation that fuels long-term learning.

### 11.6.3 Washback on Curriculum and Pedagogy

At the institutional level, the adoption of AI assessment may reshape curricula in ways that privilege assessable skills over non-assessable ones. If AI systems can reliably assess grammar, vocabulary, and reading comprehension but cannot assess pragmatic competence, intercultural communication, or critical media literacy, the curriculum may narrow to focus on what the AI can measure. This narrowing effect is well-documented in the traditional testing literature (Alderson & Wall, 1993; Au, 2007) and is amplified by AI assessment because the scope of what AI can assess is both broader (more skills can be assessed automatically) and narrower (the skills that can be assessed automatically are a subset of communicative competence) than traditional testing.

Language program administrators may face pressure to adopt AI assessment systems for their efficiency and cost-effectiveness, even when those systems do not adequately capture the learning outcomes the program values. The economic logic is powerful: an AI assessment that costs a fraction of human scoring and produces scores in real time is difficult to resist, even when the scores represent a narrower construct than the program intends. The result is a form of construct drift, in which the assessed construct gradually replaces the intended construct as the de facto goal of instruction.

---

## 11.7 Bias in AI Testing Systems

### 11.7.1 Sources of Bias

Bias in AI assessment systems can enter through multiple pathways, and identifying and mitigating these biases requires understanding each source. Drawing on Suresh and Guttag's (2021) taxonomy of machine learning bias, we can identify several types relevant to language assessment:

**Training data bias**: AI scoring models are trained on corpora of scored language samples. If the training data overrepresents certain populations (native speakers, speakers from particular L1 backgrounds, test-takers from specific socioeconomic or educational contexts), the model will learn scoring patterns that reflect those populations' characteristics as the norm. Features associated with underrepresented populations may be treated as deviant, resulting in systematically lower scores for those groups.

**Annotation bias**: The human scores used to train AI scoring models reflect the judgments of human raters, who bring their own biases to the scoring process. Research has documented systematic effects of rater L1 background, familiarity with non-native speech, and cultural assumptions on human ratings of writing and speaking proficiency (Hamp-Lyons & Davies, 2008; Winke, Gass, & Myford, 2013). These biases are encoded in the training data and reproduced by the AI system, potentially at a larger scale and with less accountability than the original human scoring.

**Feature selection bias**: The choice of linguistic features used as inputs to AI scoring models reflects assumptions about what constitutes proficiency. If the feature set emphasizes syntactic complexity, lexical sophistication, and formal accuracy--features associated with academic, standard-language registers--the scoring model will systematically advantage test-takers who have been socialized into those registers and disadvantage those who have not. This is particularly concerning for L2 speakers from non-Western educational traditions, speakers of non-standard varieties, and speakers whose communicative strengths lie in pragmatic or interactional domains rather than in formal linguistic accuracy.

**Aggregation bias**: When AI scoring models treat diverse populations as a single group, they may produce scores that are fair on average but unfair for specific subgroups. A model that performs well across the full range of proficiency levels may systematically over- or under-estimate the ability of learners at particular levels or from particular backgrounds. Disaggregated analysis by L1 background, gender, age, and educational context is essential but rarely conducted or reported for commercial AI assessment systems.

### 11.7.2 Differential Validity and Fairness

The language assessment community has developed specific frameworks for evaluating test fairness that are directly applicable to AI systems. The concept of differential item functioning (DIF) identifies test items that perform differently for groups matched on overall ability--items that are easier or harder for one group than another, controlling for proficiency level. DIF analysis can be applied to AI-scored assessments by examining whether AI scores show systematic group differences after controlling for proficiency as measured by an independent criterion.

Several studies have investigated differential validity in automated scoring. Bridgeman, Trapani, and Attali (2012) found small but statistically significant differences in e-rater scores across gender and L1 groups, with the system tending to assign higher scores to essays with more complex syntax regardless of content quality. Loukina, Madnani, and Zechner (2019) documented that automated speaking scores were less reliable for speakers from certain L1 backgrounds, with reliability degradation correlated with ASR transcription error rates. These findings suggest that AI scoring systems do not affect all populations equally and that fairness analyses should be a required component of any AI assessment validation study.

### 11.7.3 The Accountability Gap

Perhaps the most concerning aspect of bias in AI assessment is the accountability gap. When a human rater produces a biased score, the bias can, in principle, be identified through rater training, monitoring, and moderation. The rater can be retrained or removed. When an AI system produces biased scores, the bias may be difficult to identify (because it is distributed across millions of model parameters), difficult to attribute (because the model's decision process is opaque), and difficult to remediate (because retraining a model requires new data and new training infrastructure).

The opacity of AI scoring models creates what Burrell (2016) calls "opacity as the absence of interpretability": the model's decisions cannot be explained in terms that stakeholders (learners, teachers, parents, policymakers) can understand and challenge. This is particularly problematic in high-stakes assessment contexts where test-takers have a right to understand and contest their scores. The European Union's AI Act (2024) and the Council of Europe's Framework on AI (2024) both require that AI systems used in high-stakes educational decisions provide explanations for their outputs--a requirement that current AES and automated speaking assessment systems are ill-equipped to meet.

---

## 11.8 The Promise of Continuous, Embedded Assessment

### 11.8.1 Assessment Without Tests

The most radical implication of AI assessment technology is the potential elimination of discrete testing events in favor of continuous, embedded assessment. In this vision, assessment is not something that happens at the end of a unit, semester, or program; it is something that happens continuously, invisibly, as a byproduct of everyday learning activities. Every time a learner writes a sentence in an AI-powered writing tool, practices a conversation with an AI tutor, or reads an adaptive text, the system collects data about the learner's linguistic competence and updates its model of the learner's proficiency profile.

This vision has deep theoretical appeal. It eliminates the artificiality and anxiety of test situations, which may depress performance below true ability levels (especially for test-anxious learners). It provides a more representative sample of learner performance across contexts, task types, and time periods than any single test administration can achieve. It enables truly formative assessment--assessment that directly feeds back into instruction in real time rather than providing summative judgments after the learning opportunity has passed.

The concept aligns with what Mislevy, Almond, and Lukas (2003) call "evidence-centered design" (ECD), a framework that specifies how observations of learner behavior can be accumulated and combined to support inferences about unobservable competencies. In an ECD framework, every learner interaction generates "evidence" that is weighed according to the interaction's relevance to specific competency facets. An AI system that implements ECD can build a multifaceted, continuously updated competency profile from the totality of a learner's interactions, rather than relying on a single snapshot from a test event.

### 11.8.2 The Surveillance Concern

The flip side of continuous, embedded assessment is continuous surveillance. If every learner interaction is being analyzed for evidence of competency, the learner is never not being assessed. The distinction between learning time (low stakes, exploratory, error-friendly) and assessment time (high stakes, performance-focused, error-consequential) collapses, potentially transforming the entire learning environment into a panoptic assessment space.

This concern is not merely theoretical. Research on the psychological effects of surveillance in educational settings (Niemiec & Ryan, 2009; Zuboff, 2019) documents negative effects on intrinsic motivation, creativity, and risk-taking. Learners who know they are being watched perform differently--often worse--than learners who feel safe from evaluation. If continuous embedded assessment creates a perpetual state of evaluation, it may undermine the psychological safety that Krashen's (1982) Affective Filter Hypothesis and Dornyei's (2005) motivational framework identify as conducive to language acquisition.

The design challenge is to create assessment systems that are continuous and embedded but not oppressive--systems that collect data for learning improvement without creating the subjective experience of constant surveillance. This requires careful design choices about what data is collected, how it is stored and used, who has access to it, and how learners are informed and empowered to control their own data. Transparency is essential: learners should know what the system is tracking, how that data informs their learning experience, and what rights they have to opt out, correct, or delete their data.

### 11.8.3 The Integration of Assessment and Dynamic Instruction

When AI assessment is truly continuous and embedded, the boundary between assessment and instruction dissolves--and this dissolution creates the conditions for a pedagogical paradigm shift. In the traditional model, instruction and assessment are separate activities: the teacher teaches, then tests, then uses test results to plan subsequent instruction. In the AI-mediated model, assessment-instruction integration is continuous: the system assesses, instructs, reassesses, and adjusts instruction in a real-time loop.

This integration is the technological realization of Vygotsky's (1978) vision of assessment as mediation. In Vygotskian dynamic assessment, the assessor does not merely observe performance but actively intervenes to scaffold learning, and the learner's responsiveness to scaffolding becomes the assessment datum. An AI system that continuously monitors performance, provides graduated scaffolding when difficulties are detected, and tracks the learner's trajectory of improvement is performing a computational version of dynamic assessment--not merely measuring current ability but actively promoting development and measuring the rate and pattern of that development.

The realization of this vision depends on the sophistication of the AI system's pedagogical model. A system that simply repeats items the learner gets wrong is not performing dynamic assessment; it is performing drill. Genuine dynamic assessment requires the system to diagnose why the learner is struggling, provide qualitatively different levels and types of support, and distinguish between learners who need perceptual input, explicit rule explanation, additional examples, or communicative practice. Current AI systems approximate this capability for constrained domains (vocabulary, grammar, phoneme discrimination) but fall far short for complex, open-ended language tasks.

---

## 11.9 Ethical Implications of AI Assessment at Scale

### 11.9.1 Consequential Validity Revisited

Messick's (1989) concept of consequential validity--the requirement that the social consequences of assessment use be considered as part of the validity argument--takes on particular urgency in the context of AI assessment at scale. When AI assessment systems are deployed to millions of learners simultaneously, the consequences of even small systematic biases are amplified enormously. A scoring algorithm that underestimates the proficiency of learners from a particular L1 background by 0.3 standard deviations--a difference that might be considered negligible in a single assessment event--translates into thousands of misplacements, denied opportunities, and reinforced inequities when applied across an entire population.

The scale of AI assessment also creates new categories of consequence. When assessment data is stored indefinitely in cloud databases, learners' linguistic errors, learning trajectories, and proficiency profiles become permanent digital records. These records may be accessed by educational institutions, employers, or immigration authorities for purposes far removed from their original assessment context. The "data trail" of AI-mediated assessment raises questions about learner privacy, data ownership, and the right to be forgotten that the traditional assessment paradigm--in which test papers were physical documents that could be shredded--did not face.

### 11.9.2 Informed Consent and Transparency

The ethical deployment of AI assessment requires informed consent--learners must understand what is being assessed, how their data will be used, and what the consequences of assessment outcomes may be. In practice, informed consent for AI assessment is often nominal: learners click through terms of service agreements they do not read, for systems whose scoring mechanisms they cannot inspect, with consequences they cannot fully anticipate.

True informed consent requires transparency about the AI system's operation: what features it evaluates, what norms it applies, what populations it was trained on, what its known biases are, and what limitations its developers acknowledge. The Language Testing Research Colloquium (LTRC) and the International Language Testing Association (ILTA) have developed codes of ethics and guidelines for fair testing practices (ILTA, 2018) that should be extended to cover AI-specific concerns. At minimum, any AI assessment system used for high-stakes decisions should be required to provide a publicly available technical report documenting its validation evidence, bias analyses, and known limitations.

### 11.9.3 The Human-in-the-Loop Imperative

For high-stakes assessment decisions--university admissions, professional certification, immigration and asylum processes--the ethical case for maintaining human oversight of AI scoring is compelling. A "human-in-the-loop" model, in which AI scoring is used as one input to human decision-making rather than as the sole determinant of outcomes, preserves the accountability that automated scoring cannot provide. The human decision-maker can consider contextual factors, exercise professional judgment, and be held responsible for the decision in ways that an algorithm cannot.

The practical challenge is designing human-in-the-loop systems that genuinely preserve human judgment rather than creating "automation bias"--the documented tendency for humans to defer to algorithmic recommendations even when those recommendations are incorrect (Parasuraman & Riley, 1997). Research on human-AI collaboration in assessment suggests that raters who see AI scores before producing their own ratings are influenced by those scores, even when they disagree (Ramanarayanan, Siniscalchi, Suendermann-Oeft, & Lange, 2022). Effective human-in-the-loop design may require presenting human raters with AI-generated information (error analyses, feature profiles) without revealing the AI's holistic score, allowing the human to form an independent judgment supported by, but not determined by, algorithmic analysis.

### 11.9.4 Assessment Equity in the Age of AI

The deployment of AI assessment intersects with broader questions of educational equity. Learners from well-resourced backgrounds have access to AI-powered test preparation tools that can analyze their performance, identify weaknesses, and provide targeted practice--tools that are expensive, require digital access, and assume familiarity with AI interfaces. Learners from under-resourced backgrounds may face AI assessments without having had access to the AI-mediated practice environments that prepare others for this format. The result is a new dimension of the digital divide (Warschauer, 2003): a gap not only in access to technology but in access to the AI-specific preparation that shapes performance on AI-mediated assessments.

Furthermore, the global deployment of AI assessment systems developed primarily in Western, English-dominant contexts raises concerns about cultural and linguistic imperialism. An AI scoring model trained on writing samples from American universities may encode assumptions about argumentation, evidence, and rhetorical structure that reflect Western academic conventions rather than universal standards of communicative competence. When this model is used to assess learners in East Asian, African, or Latin American educational contexts, it may systematically disadvantage rhetorical traditions that organize argumentation differently, value different types of evidence, or employ different discourse conventions.

---

## 11.10 Toward Responsible AI Assessment: Principles and Practices

### 11.10.1 A Framework for Evaluating AI Assessment Systems

Drawing on the analysis in this chapter, we can articulate a set of principles for the responsible evaluation and deployment of AI assessment in language education:

**Principle 1: Construct fidelity.** AI assessment systems should be evaluated against clearly articulated construct definitions, and the gap between the intended construct and the assessed construct should be explicitly acknowledged. If an AI system assesses grammar, vocabulary, and fluency but not pragmatic competence or sociolinguistic appropriateness, this limitation should be stated in all score reports and decision-making contexts.

**Principle 2: Bias auditing.** AI assessment systems should undergo regular, independent bias audits examining differential performance across L1 backgrounds, genders, ages, and socioeconomic groups. The results of these audits should be publicly available.

**Principle 3: Transparency.** The features used for scoring, the norms against which performance is evaluated, and the populations on which the system was trained should be documented and accessible to stakeholders.

**Principle 4: Human oversight for high stakes.** AI scoring should not be the sole basis for high-stakes decisions. Human judgment must be preserved in the decision loop for assessments with significant consequences for learners' educational or professional trajectories.

**Principle 5: Learner agency.** Learners should have the right to understand their AI-generated scores, to challenge scores they believe are inaccurate, and to have their work re-evaluated by a human assessor. Assessment systems that do not provide these rights should not be used for consequential decisions.

**Principle 6: Washback monitoring.** The effects of AI assessment on teaching and learning should be monitored longitudinally, with particular attention to whether AI assessment narrows curricula, reduces pedagogical creativity, or orients instruction toward algorithmically rewarded features at the expense of broader communicative goals.

### 11.10.2 The Assessment-Learning Integration Imperative

The chapter's central argument is that AI assessment's greatest potential lies not in making existing tests cheaper and faster but in fundamentally reconceiving the relationship between assessment and learning. When assessment becomes continuous, embedded, and formative--when it serves learning rather than judging it--the entire educational paradigm shifts. Dynamic assessment, individualized learning trajectories, and real-time adaptation become possible at a scale that human-only assessment cannot achieve.

Realizing this potential requires abandoning the assumption that assessment and instruction are separate activities with separate purposes. It requires designing AI systems that assess in order to teach, not just teach in order to assess. And it requires maintaining the ethical safeguards--transparency, fairness, human oversight, learner agency--that prevent continuous assessment from becoming continuous surveillance.

The technology exists to create language assessment systems that are more valid (because they sample performance across contexts and time), more fair (because they can adapt to individual backgrounds and needs), and more useful (because they feed directly into personalized instruction) than any static test. Whether this potential is realized depends on whether the field of language assessment can maintain its commitment to validity, fairness, and consequential accountability in the face of the efficiency pressures and commercial incentives that drive AI adoption.

---

## 11.11 Conclusion

AI is transforming language assessment along multiple fronts: automated essay scoring evaluates writing at scale, automated speech assessment extends the paradigm to spoken language, computer-adaptive testing optimizes measurement precision, and learning analytics enable continuous, embedded assessment. Each of these technologies offers genuine affordances--efficiency, consistency, immediacy, adaptability--that address real limitations of human-only assessment.

Yet each technology also carries significant risks. Automated essay scoring measures surface features of text rather than the communicative and rhetorical competence it claims to assess. Automated speech assessment propagates ASR errors inequitably across speaker populations. Adaptive testing may narrow the construct to what can be efficiently measured. And continuous embedded assessment threatens to transform every learning moment into an assessment event, with consequences for learner motivation, risk-taking, and autonomy.

The path forward is neither wholesale adoption nor wholesale rejection but principled integration: deploying AI assessment where it genuinely serves learning, maintaining human judgment where stakes are high, auditing for bias systematically, and preserving the transparency and accountability that assessment validity requires. The field of language assessment has spent decades developing the theoretical and ethical frameworks needed to evaluate testing practices. Those frameworks are more needed than ever in the age of AI, not because AI assessment is inherently inferior to human assessment but because AI assessment operates at a scale, speed, and opacity that amplify both its benefits and its harms.

For the language educator, the imperative is to resist the allure of assessment automation for its own sake and to ask, always, the questions that Bachman and Palmer (2010) posed for any assessment: Is it valid? Is it fair? Is it useful? Does it serve the learner? These questions do not change because the assessor is an algorithm rather than a human. But the difficulty of answering them increases substantially--and the consequences of failing to ask them escalate with every learner whose educational trajectory is shaped by an AI system's score.

---

## References

Alderson, J. C., & Wall, D. (1993). Does washback exist? *Applied Linguistics*, *14*(2), 115-129.

Attali, Y., & Burstein, J. (2006). Automated essay scoring with e-rater V.2. *Journal of Technology, Learning, and Assessment*, *4*(3), 1-31.

Au, W. (2007). High-stakes testing and curricular control: A qualitative metasynthesis. *Educational Researcher*, *36*(5), 258-267.

Bachman, L. F., & Palmer, A. S. (1996). *Language testing in practice: Designing and developing useful language tests*. Oxford University Press.

Bachman, L. F., & Palmer, A. S. (2010). *Language assessment in practice*. Oxford University Press.

Black, P., & Wiliam, D. (1998). Assessment and classroom learning. *Assessment in Education: Principles, Policy & Practice*, *5*(1), 7-74.

Bridgeman, B., Trapani, C., & Attali, Y. (2012). Comparison of human and machine scoring of essays: Differences by gender, ethnicity, and country. *Applied Measurement in Education*, *25*(1), 27-40.

Burrell, J. (2016). How the machine "thinks": Understanding opacity in machine learning algorithms. *Big Data & Society*, *3*(1), 1-12.

Cheng, L. (2005). *Changing language teaching through language testing: A washback study*. Cambridge University Press.

Council of Europe. (2001). *Common European Framework of Reference for Languages: Learning, teaching, assessment*. Cambridge University Press.

Deane, P. (2013). On the relation between automated essay scoring and modern views of the writing construct. *Assessing Writing*, *18*(1), 7-24.

Dornyei, Z. (2005). *The psychology of the language learner: Individual differences in second language acquisition*. Lawrence Erlbaum.

Ericsson, P. F., & Haswell, R. H. (Eds.). (2006). *Machine scoring of student essays: Truth and consequences*. Utah State University Press.

Foucault, M. (1977). *Discipline and punish: The birth of the prison* (A. Sheridan, Trans.). Vintage.

Ginther, A., Dimova, S., & Yang, R. (2010). Conceptual and empirical relationships between temporal measures of fluency and oral English proficiency. *Language Testing*, *27*(3), 379-399.

Hamp-Lyons, L., & Davies, A. (2008). The Englishes of English tests: Bias revisited. *World Englishes*, *27*(1), 26-39.

Hattie, J. (2009). *Visible learning: A synthesis of over 800 meta-analyses relating to achievement*. Routledge.

ILTA (International Language Testing Association). (2018). *ILTA guidelines for practice*. https://www.iltaonline.com/page/ILTAGuidelinesForPractice

Krashen, S. D. (1982). *Principles and practice in second language acquisition*. Pergamon Press.

LaFlair, G. T., & Egbert, J. (2022). A validity argument for the Duolingo English Test. *Language Testing*, *39*(4), 502-527.

Landauer, T. K., Laham, D., & Foltz, P. W. (2003). Automated scoring and annotation of essays with the Intelligent Essay Assessor. In M. D. Shermis & J. Burstein (Eds.), *Automated essay scoring: A cross-disciplinary perspective* (pp. 87-112). Lawrence Erlbaum.

Lantolf, J. P., & Poehner, M. E. (2004). Dynamic assessment of L2 development: Bringing the past into the future. *Journal of Applied Linguistics*, *1*(1), 49-72.

Lantolf, J. P., & Poehner, M. E. (2011). Dynamic assessment in the classroom: Vygotskian praxis for second language development. *Language Teaching Research*, *15*(1), 11-33.

Lantolf, J. P., & Poehner, M. E. (2014). *Sociocultural theory and the pedagogical imperative in L2 education: Vygotskian praxis and the research/practice divide*. Routledge.

Loukina, A., Madnani, N., & Zechner, K. (2019). The many dimensions of algorithmic fairness in educational applications. In *Proceedings of the Fourteenth Workshop on Innovative Use of NLP for Building Educational Applications* (pp. 1-10).

McNamara, T. (2000). *Language testing*. Oxford University Press.

Messick, S. (1989). Validity. In R. L. Linn (Ed.), *Educational measurement* (3rd ed., pp. 13-103). American Council on Education/Macmillan.

Mislevy, R. J., Almond, R. G., & Lukas, J. F. (2003). A brief introduction to evidence-centered design. *ETS Research Report Series*, *2003*(1), i-29.

Niemiec, C. P., & Ryan, R. M. (2009). Autonomy, competence, and relatedness in the classroom: Applying self-determination theory to educational practice. *Theory and Research in Education*, *7*(2), 133-144.

Parasuraman, R., & Riley, V. (1997). Humans and automation: Use, misuse, disuse, abuse. *Human Factors*, *39*(2), 230-253.

Perelman, L. (2014). When "the state of the art" is counting words. *Assessing Writing*, *21*, 104-111.

Ramanarayanan, V., Siniscalchi, S. M., Suendermann-Oeft, D., & Lange, P. (2022). Human-AI collaboration in automated scoring: A review. *Language Assessment Quarterly*, *19*(3), 278-299.

Rea-Dickins, P. (2001). Mirror, mirror on the wall: Identifying processes of classroom assessment. *Language Testing*, *18*(4), 429-462.

Shohamy, E. (2001). *The power of tests: A critical perspective on the uses of language tests*. Pearson.

Siemens, G. (2013). Learning analytics: The emergence of a discipline. *American Behavioral Scientist*, *57*(10), 1380-1400.

Suresh, H., & Guttag, J. (2021). A framework for understanding sources of harm throughout the machine learning life cycle. In *Equity and Access in Algorithms, Mechanisms, and Optimization* (pp. 1-9). ACM.

Swain, M. (1985). Communicative competence: Some roles of comprehensible input and comprehensible output in its development. In S. Gass & C. Madden (Eds.), *Input in second language acquisition* (pp. 235-253). Newbury House.

Ushioda, E. (2009). A person-in-context relational view of emergent motivation, self and identity. In Z. Dornyei & E. Ushioda (Eds.), *Motivation, language identity and the L2 self* (pp. 215-228). Multilingual Matters.

Vygotsky, L. S. (1978). *Mind in society: The development of higher psychological processes*. Harvard University Press.

Wainer, H., Dorans, N. J., Flaugher, R., Green, B. F., Mislevy, R. J., Steinberg, L., & Thissen, D. (2000). *Computerized adaptive testing: A primer* (2nd ed.). Lawrence Erlbaum.

Wang, Y., Shang, H., Liou, H., Shih, C., & Chen, H. (2023). Automated essay scoring using pre-trained language models: A systematic review. *Computer Assisted Language Learning*, *36*(5-6), 832-858.

Warschauer, M. (2003). *Technology and social inclusion: Rethinking the digital divide*. MIT Press.

Warschauer, M., & Grimes, D. (2008). Automated writing assessment in the classroom. *Pedagogies: An International Journal*, *3*(1), 22-36.

Weigle, S. C. (2013). English as a second language writing and automated essay evaluation. In M. D. Shermis & J. Burstein (Eds.), *Handbook of automated essay evaluation* (pp. 36-54). Routledge.

Winke, P., Gass, S., & Myford, C. (2013). Raters' L2 background as a potential source of bias in rating oral performance. *Language Testing*, *30*(2), 231-252.

Xi, X. (2010). Automated scoring and feedback systems: Where are we and where are we heading? *Language Testing*, *27*(3), 291-300.

Yan, D., & Chung, E. (2023). Can automated scoring distinguish AI-generated text from human writing? Implications for writing assessment. *Educational Measurement: Issues and Practice*, *42*(3), 15-28.

Zuboff, S. (2019). *The age of surveillance capitalism: The fight for a human future at the new frontier of power*. PublicAffairs.

---

*Discussion Questions*

1. Messick (1989) argued that the social consequences of assessment use must be considered as part of the validity argument. What specific social consequences should be examined for an AI-powered language placement test used by a university to sort incoming international students into proficiency levels?

2. Consider the "assessment without tests" vision described in Section 11.8. What are the potential benefits for learners who experience test anxiety? What safeguards would be necessary to prevent continuous embedded assessment from becoming continuous surveillance?

3. Perelman (2014) demonstrated that gibberish essays could receive high scores from automated essay scoring systems. What does this reveal about the construct validity of AES? How should this finding influence the deployment of AES in L2 writing assessment?

4. The Duolingo English Test was designed from the ground up for AI scoring, rather than adapting human-scored assessments for AI. What are the advantages and risks of this "AI-native" approach to assessment design? Does the construct change when the assessment is designed around the technology's capabilities?

5. Design a hybrid human-AI assessment system for a university intensive English program that leverages AI for continuous formative assessment while preserving human judgment for summative decisions. What role would the AI play? What role would the teacher play? Where would the boundaries be drawn?

6. How might the deployment of Western-developed AI assessment systems in non-Western educational contexts constitute a form of linguistic imperialism? What steps could be taken to develop culturally responsive AI assessment?
