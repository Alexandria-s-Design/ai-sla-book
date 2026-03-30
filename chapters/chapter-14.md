# Chapter 14: Research Methods for AI-SLA Studies

---

## 14.1 Introduction: The Methodological Imperative

The integration of artificial intelligence into second language acquisition contexts has created a methodological crisis of opportunity. On one hand, AI systems generate unprecedented quantities of data about language learning processes — every keystroke, every pause, every revision, every conversational turn captured in digital logs that dwarf the observational capabilities of any human researcher. On the other hand, the very properties that make AI systems powerful — their complexity, their opacity, their capacity for personalization, their rapid evolution — introduce methodological challenges that existing SLA research paradigms were not designed to address.

This chapter provides a comprehensive guide to research methodology for scholars investigating AI-mediated second language acquisition. It does not attempt to reinvent the methodological wheel; the rich traditions of quantitative, qualitative, and mixed-methods research in SLA (Gass & Mackey, 2012; Duff, 2008; Plonsky & Gass, 2011) remain foundational. Rather, it examines how established methodological approaches must be adapted, extended, and in some cases supplemented to address the unique characteristics of AI-mediated language learning environments. The chapter also addresses the emerging role of learning analytics and big data in SLA research, the ethical dimensions of AI research with language learners, and the reproducibility challenges posed by rapidly evolving commercial AI systems.

The need for rigorous, theoretically grounded methodology in AI-SLA research cannot be overstated. The field is awash in practitioner reports, product reviews, and small-scale classroom studies that, while valuable as preliminary explorations, lack the methodological rigor necessary to advance theoretical understanding or inform policy. Published studies frequently suffer from inadequate control conditions, conflation of novelty effects with genuine learning gains, failure to operationalize theoretical constructs, and insufficient attention to the ecological validity of experimental tasks. If AI-SLA is to mature as a field of scholarly inquiry rather than a collection of anecdotal technology reviews, a commitment to methodological excellence is essential.

---

## 14.2 Fundamental Methodological Challenges in AI-SLA Research

### 14.2.1 The Moving Target Problem

Perhaps the most distinctive methodological challenge in AI-SLA research is that the object of study is in constant flux. Commercial AI systems — the platforms that millions of language learners actually use — are updated frequently, sometimes multiple times per month. A study conducted on GPT-4 in January may not be replicable on the same model in March, because the model's weights, safety filters, or system prompts may have been modified by the provider. A study of Duolingo's AI-powered speaking exercises may find different results after a platform update that changes the underlying speech recognition engine or feedback algorithm.

This "moving target" problem has no perfect solution, but several mitigation strategies are available. First, researchers should document the exact version and configuration of any AI system used in a study, including model version numbers, API endpoints, system prompt configurations, and dates of data collection. Second, where possible, researchers should use open-source models that can be frozen at a specific version (e.g., LLaMA, Mistral) rather than commercial APIs that may change without notice. Third, researchers can archive the AI system's outputs at the time of data collection, creating a record of system behavior that can be compared to later versions even if the system itself has changed.

Chapelle (2001) argued that CALL evaluation must attend to both the technology and the learning context. In the AI era, this means that methodological descriptions must specify not just "participants used ChatGPT" but the exact model, temperature setting, system prompt (if customized), date of interaction, and any other parameters that could affect the AI's behavior. Without this level of specification, replication is impossible and cross-study comparison is meaningless.

### 14.2.2 The Personalization Paradox

AI systems that adapt to individual learners — adjusting content difficulty, feedback type, interaction style, and pacing based on learner performance — create a fundamental methodological tension. The adaptive capability is precisely what makes AI pedagogically promising: the system provides each learner with a different experience tailored to their needs. But this same capability undermines experimental control, because no two participants in a study receive the same treatment.

In traditional experimental designs, the treatment condition is held constant across participants. All learners in the experimental group receive the same materials, the same feedback, and the same interaction conditions, allowing the researcher to attribute between-group differences to the treatment. When the AI personalizes the treatment for each learner, the treatment is no longer a single entity but a family of related experiences — and the researcher must decide how to conceptualize and analyze this variability.

Several approaches to this challenge have been proposed. Randomized controlled trials (RCTs) can compare adaptive AI conditions to non-adaptive AI conditions or to human-delivered instruction, treating the adaptive system as a "black box" and measuring outcomes without attempting to control the treatment's internal variability (cf. medical trial methodology for personalized treatments). Alternatively, researchers can log the AI's adaptive decisions for each participant and include these as covariates or moderating variables in the analysis, effectively treating the AI's personalization as data rather than noise.

A third approach draws on design-based research (DBR) methodology (Collins, Joseph, & Bielaczyc, 2004), which embraces the complexity of real learning environments rather than attempting to control it away. In DBR, the adaptive AI system is iteratively designed, deployed, studied, and refined, with each cycle generating both practical improvements and theoretical insights. This approach sacrifices the internal validity of controlled experiments in favor of ecological validity and design knowledge — a tradeoff that may be appropriate for a field where the technology is evolving faster than experimental studies can be conducted.

### 14.2.3 The Construct Definition Challenge

AI systems challenge researchers to define their constructs with greater precision than may previously have been necessary. Consider "corrective feedback," a construct central to SLA theory and to many AI applications (see Chapter 7). In human interaction, corrective feedback encompasses recasts, prompts, explicit correction, metalinguistic explanation, and various combinations thereof, all embedded in social relationships with their attendant power dynamics, affective dimensions, and implicit social contracts. When an AI system provides corrective feedback, which of these dimensions are preserved and which are absent?

The answer has methodological implications. A study comparing "AI corrective feedback" to "human corrective feedback" must specify what counts as feedback in each condition and acknowledge the dimensions on which the two differ. If the AI provides metalinguistic explanations while the human tutor tends to provide recasts, the study is not comparing "AI vs. human feedback" but "explicit metalinguistic feedback vs. recasts" — a comparison for which existing SLA research already provides substantial evidence (Lyster & Ranta, 1997; Li, 2010). Without precise construct definition, researchers risk attributing to "AI" what is actually attributable to a specific feedback type or instructional approach that happens to be implemented through AI.

This challenge extends to virtually every SLA construct discussed in this book: input (is AI-generated text "authentic" input?), interaction (is AI conversation "genuine" negotiation of meaning?), output (does AI-scaffolded writing constitute "pushed output"?), and identity (does interacting with AI create "investment" in the target language community?). Each of these constructs must be operationalized with attention to how AI mediation may alter the construct's theoretical meaning.

### 14.2.4 The Ecological Validity Dilemma

Laboratory studies of AI-SLA interactions risk poor ecological validity because they typically constrain learners' use of AI in ways that do not reflect actual practice. In real life, learners who use AI for language learning do not limit themselves to a single tool, a single language skill, or a pre-defined task sequence. They switch between ChatGPT, Google Translate, Duolingo, and YouTube in a single study session, using each tool for different purposes and in different ways. They use AI while simultaneously texting friends, listening to music, and monitoring social media — the multitasking reality of contemporary digital life.

Laboratory studies that isolate a single AI tool, a single language skill, and a single interaction modality capture a slice of this reality but may miss the emergent properties of the ecosystem. A learner who uses ChatGPT for grammar questions, Duolingo for vocabulary, and an AI pronunciation app for speaking may develop different competencies than one who uses only ChatGPT, but this ecosystem effect is invisible to single-tool studies.

Conversely, naturalistic studies that observe learners using AI in their everyday contexts face the challenge of confounds — when learners use multiple tools and strategies, it is difficult to attribute any observed learning gains to a specific AI interaction. The methodological literature on complex interventions in health and education (Craig et al., 2008) offers some guidance, but the AI-SLA field has not yet systematically adopted these approaches.

---

## 14.3 Quantitative Approaches

### 14.3.1 Experimental and Quasi-Experimental Designs

True experimental designs with random assignment remain the gold standard for establishing causal relationships between AI interventions and learning outcomes. The prototypical design compares an AI-assisted treatment group to a control group that receives either (a) no technology, (b) non-AI technology, or (c) a different AI tool or configuration. Pre-tests and post-tests measure learning gains, and statistical analyses determine whether between-group differences are significant.

Several design considerations are specific to AI-SLA experiments. First, the choice of control condition requires careful thought. A "no technology" control is often criticised as a straw man, since any technology will likely produce benefits over none. A more informative comparison pits the AI intervention against the most effective available alternative — whether that is human tutoring, traditional CALL materials, or a different AI tool. This "active control" design (Boot et al., 2013) provides evidence about the AI's added value rather than merely its superiority to doing nothing.

Second, researchers must attend to novelty effects. Participants who use AI for language learning for the first time may exhibit heightened motivation, engagement, and effort — the so-called "Hawthorne effect" — that inflates short-term learning gains. Longitudinal designs that extend beyond the novelty period (typically three to four weeks of initial use) provide more valid estimates of AI's sustained impact on learning.

Third, sample size considerations are critical. Plonsky (2013) demonstrated that many SLA studies are underpowered, with sample sizes insufficient to detect small or medium effects. AI-SLA studies face this challenge acutely because the individual variability introduced by adaptive AI systems increases within-group variance, requiring larger samples to achieve adequate power. Power analyses should be conducted a priori, and researchers should consider multi-site studies to achieve adequate sample sizes.

A robust experimental design for an AI-SLA study might take the following form: a pre-registered, multi-site randomized controlled trial comparing an AI chatbot for conversation practice (treatment) to matched human-human conversation practice (active control) over a 12-week period, with pre-test, mid-test, and post-test assessments of oral proficiency (rated by blinded human evaluators using a validated rubric), with AI interaction logs analyzed to identify dose-response relationships and moderating variables (learner proficiency level, L1 background, prior technology experience). This design is demanding — and largely absent from the current literature — but represents the level of rigor the field needs.

### 14.3.2 Quasi-Experimental Designs

In many educational contexts, true randomization is impossible due to institutional constraints (e.g., students are already assigned to classes), ethical concerns (e.g., withholding a potentially beneficial intervention from the control group), or practical limitations (e.g., insufficient participant numbers for random assignment). Quasi-experimental designs that compare intact groups — different class sections, different schools, or different cohorts — provide a pragmatic alternative.

The most common quasi-experimental design in AI-SLA research is the pretest-posttest nonequivalent groups design, in which two existing class sections receive different conditions. This design is vulnerable to selection bias (the groups may differ in ways that affect outcomes), and researchers should employ statistical techniques to address this threat. Propensity score matching, analysis of covariance with pre-test scores as covariates, and difference-in-differences analysis can partially mitigate selection bias, though they cannot eliminate it entirely.

A particularly useful quasi-experimental approach for AI-SLA research is the crossover design, in which each group serves as both treatment and control at different time points. Group A uses the AI tool for vocabulary learning in weeks 1-6 while Group B uses traditional methods; in weeks 7-12, the conditions are reversed. This within-subjects component reduces the impact of individual differences and addresses the ethical concern of withholding the treatment, since all participants eventually receive it.

### 14.3.3 Statistical Approaches for AI-Adaptive Environments

Standard statistical approaches assume that all participants in a treatment condition receive the same treatment. When AI systems personalize the treatment, this assumption is violated. Several statistical approaches can accommodate this complexity.

Mixed-effects models (also called multilevel models or hierarchical linear models) are particularly well-suited to AI-SLA data because they can model multiple levels of nesting: individual observations nested within learners, learners nested within classes, and classes nested within schools. They can also incorporate time-varying covariates, allowing the researcher to model how AI system behavior (e.g., difficulty level, feedback frequency) changes over time and how these changes relate to learning outcomes.

Growth curve modeling extends mixed-effects models to explicitly model learning trajectories over time. Rather than comparing pre-test and post-test means, growth curve models estimate the shape of each learner's learning trajectory (linear, curvilinear, plateauing) and test whether AI conditions produce different trajectory shapes. This approach is particularly valuable for AI-SLA research because it captures the dynamic, non-linear nature of language development — a central tenet of Complex Dynamic Systems Theory (Larsen-Freeman & Cameron, 2008).

Bayesian statistical methods offer another promising approach. Unlike frequentist methods that yield only accept/reject decisions about null hypotheses, Bayesian analysis provides probability distributions over parameter values, allowing researchers to make nuanced claims about the magnitude and uncertainty of effects. Bayesian methods also handle small samples more gracefully than frequentist approaches, a practical advantage given the difficulty of recruiting large samples for intensive language learning studies. Furthermore, Bayesian meta-analytic methods can synthesize evidence across studies with different designs and measures, accumulating evidence about AI-SLA effects even when individual studies are small.

### 14.3.4 Learning Analytics and Big Data

The digital traces generated by AI language learning systems — interaction logs, keystroke data, revision histories, time-on-task measurements, navigation patterns — constitute a form of big data that can be analyzed using learning analytics methods. Learning analytics (LA) applies data science techniques to educational data with the goal of understanding and improving learning processes and outcomes (Siemens & Baker, 2012).

Several LA methods are particularly relevant to AI-SLA research. Sequence mining identifies common patterns in learners' interaction sequences — for example, the typical sequence of actions a learner follows when receiving corrective feedback from an AI, or the order in which learners access different features of an AI learning platform. These patterns can reveal how learners actually use AI tools, often in ways that differ substantially from how designers intended the tools to be used.

Clustering algorithms can identify groups of learners with similar interaction patterns, potentially revealing learner typologies that correspond to different levels of benefit from AI instruction. For instance, cluster analysis might reveal that learners who alternate between AI conversation practice and explicit grammar study sessions show different learning trajectories than learners who exclusively use conversation practice — a finding with implications for pedagogical guidance.

Natural language processing applied to learner-AI interaction transcripts can automate the analysis of linguistic features at scale. Complexity, accuracy, and fluency (CAF) metrics — the standard measures of L2 development — can be computed automatically for thousands of writing samples or conversation turns, enabling researchers to track linguistic development at a granularity impossible with manual analysis. Tools such as TAALES (Kyle & Crossley, 2015), L2SCA (Lu, 2010), and newer LLM-based analysis methods can process learner output to quantify syntactic complexity, lexical sophistication, accuracy rates, and fluency indicators.

However, learning analytics approaches carry significant limitations. The data captured by AI systems reflects only the dimensions that the system was designed to track — typically quantifiable behaviors such as time, clicks, and text. Motivational states, identity processes, social dynamics, and the subjective experience of learning are largely invisible in log data. The risk is that LA-driven research overemphasizes measurable behaviors at the expense of the cognitive, social, and affective dimensions of SLA that give those behaviors meaning.

---

## 14.4 Qualitative Approaches

### 14.4.1 Case Study Research

Case study methodology — the intensive investigation of a single case or small number of cases — offers rich opportunities for understanding AI-mediated SLA in its full complexity. Duff (2008, 2014) articulated criteria for rigorous case study research in applied linguistics, emphasizing the importance of prolonged engagement, multiple data sources, systematic analysis, and reflexive interpretation. These criteria apply with equal force to AI-SLA case studies.

A well-designed case study of AI-mediated language learning might follow a single learner or a small group of learners over an extended period (a semester or academic year), collecting multiple types of data: AI interaction logs, stimulated recall interviews (in which learners review recordings of their AI interactions and comment on their thought processes), periodic proficiency assessments, learner journals or reflective blogs, classroom observations, and interviews with the learner's teacher or tutor.

The strength of case study research lies in its capacity to capture the holistic experience of learning with AI — including the cognitive, social, affective, and identity dimensions that quantitative measures may miss. A case study might reveal, for example, that a learner's initial enthusiasm for AI conversation practice wanes after several weeks because the predictability of AI responses fails to create the social motivation that characterizes human interaction. Or it might reveal that a heritage language learner uses AI translation tools strategically to navigate between home and academic registers — a practice invisible in quantitative assessments but central to the learner's multilingual development.

### 14.4.2 Ethnographic Approaches

Ethnographic research — characterized by prolonged immersion, participant observation, and thick description (Geertz, 1973) — is well-suited to investigating how AI tools become embedded in the social and cultural practices of language learning communities. While full ethnography requires extended fieldwork that may be impractical for many researchers, ethnographically informed approaches that draw on observational methods, field notes, and cultural interpretation can provide valuable insights into AI-SLA phenomena.

Ethnographic approaches are particularly appropriate for studying how AI tools are appropriated by language learning communities in ways that may diverge from their intended use. Thorne (2003) demonstrated that technology-mediated communication tools take on meaning within specific "cultures of use" that shape how participants understand and engage with the technology. An AI chatbot designed for grammar practice might be appropriated by learners as an identity exploration tool (asking the AI questions about cultural practices, testing whether the AI recognizes their home dialect) or as a social substitute (conversing with the AI about personal topics in the target language because human conversation partners are unavailable).

Digital ethnography (Hine, 2015; Pink et al., 2016) extends ethnographic methods to online and hybrid environments. For AI-SLA research, this might involve observing and analyzing learners' interactions in online forums where they discuss their experiences with AI language tools, studying YouTube or TikTok communities that share AI language learning strategies, or conducting virtual participant observation in language learning Discord servers where AI bots are integrated into community practice.

### 14.4.3 Discourse Analysis

Discourse analysis — the systematic examination of language in use — provides powerful tools for analyzing AI-learner interactions. Several traditions within discourse analysis are relevant to AI-SLA research.

Conversation analysis (CA), with its fine-grained attention to turn-taking, repair, and sequential organization, can reveal how AI-learner conversations differ structurally from human-human conversations. Heritage and Atkinson's (1984) foundational work on institutional talk suggests that AI-learner interaction may constitute a new form of institutional discourse with its own characteristic patterns of turn allocation, topic management, and repair. Preliminary CA studies of AI-learner interaction have identified distinctive features including extended learner turns (the AI's patience encourages longer utterances), self-initiated repair prompted by AI feedback, and the absence of genuine comprehension breakdowns (since the AI can process virtually any learner input) that paradoxically reduces negotiation of meaning opportunities (Wong & Waring, 2023).

Critical discourse analysis (CDA) can examine the power dynamics and ideological assumptions embedded in AI-learner interactions. Fairclough's (1992) framework for analyzing discourse as social practice invites attention to how AI systems position learners — as deficient users who need correction, as consumers who need content, or as autonomous agents who need scaffolding. The language an AI system uses to deliver feedback (e.g., "That's incorrect. The correct form is..." vs. "Good try! A more natural way to say that would be...") encodes specific ideologies of learning, authority, and the learner-tool relationship that CDA can make visible.

Multimodal discourse analysis extends the analytical lens beyond text to encompass the visual, auditory, and interactive dimensions of AI-learner interaction. AI language learning platforms employ color, animation, sound effects, gamification elements, and spatial layout to communicate meaning and direct learner attention. Kress and van Leeuwen's (2001) social semiotic approach to multimodal analysis provides tools for examining how these non-linguistic semiotic resources interact with linguistic content to create the total learning experience.

---

## 14.5 Mixed Methods for Complex AI Learning Environments

### 14.5.1 The Case for Mixed Methods in AI-SLA Research

The complexity of AI-mediated language learning environments argues strongly for mixed-methods research designs that combine quantitative and qualitative approaches. Quantitative methods can establish whether AI interventions produce measurable learning gains across populations; qualitative methods can illuminate how those gains (or their absence) are experienced by individual learners and why some learners benefit more than others.

Creswell and Plano Clark's (2018) typology of mixed-methods designs provides a useful framework. The explanatory sequential design, in which quantitative data collection and analysis is followed by qualitative data collection to explain quantitative findings, is well-suited to AI-SLA research. For example, a researcher might conduct a quasi-experimental study comparing AI tutoring to human tutoring, then conduct interviews with selected high-performing and low-performing participants from each condition to understand the mechanisms underlying the quantitative results.

The convergent parallel design, in which quantitative and qualitative data are collected simultaneously and then integrated during interpretation, is valuable for capturing the multi-dimensional nature of AI-mediated learning. Quantitative measures of proficiency gains, combined with qualitative analysis of learner journals and AI interaction transcripts, can provide a more complete picture than either approach alone.

### 14.5.2 Design-Based Research

Design-based research (DBR) merits special attention in the AI-SLA context because it addresses a fundamental challenge: the field needs not only to study existing AI tools but also to design better ones, and the design process itself generates theoretical insights. Collins, Joseph, and Bielaczyc (2004) defined DBR as "a systematic but flexible methodology aimed to improve educational practices through iterative analysis, design, development, and implementation, based on collaboration among researchers and practitioners in real-world settings."

A DBR study of AI-assisted writing feedback might proceed through multiple iterations. Iteration 1: Deploy an LLM-based writing tutor with a specific feedback strategy (e.g., Socratic questioning) and collect data on learner interactions, learning outcomes, and learner perceptions. Analysis reveals that learners at lower proficiency levels become frustrated by the Socratic approach and disengage. Iteration 2: Redesign the system to provide more explicit feedback for lower-proficiency learners and more Socratic feedback for advanced learners, and study the effects of this adaptive approach. Analysis reveals improved engagement but inconsistent learning gains due to the AI occasionally providing incorrect metalinguistic explanations. Iteration 3: Add a verification layer that checks the AI's explanations against a grammar reference database before presenting them to learners.

Each iteration produces both a better tool and theoretical insights: in this hypothetical example, about the interaction between proficiency level and feedback type (relevant to the corrective feedback literature reviewed in Chapter 7), about learner tolerance for ambiguity in AI-generated explanations (relevant to Schmidt's Noticing Hypothesis), and about the reliability of LLM-generated metalinguistic knowledge (relevant to the "stochastic parrots" debate discussed in Chapter 3).

### 14.5.3 Action Research

Action research — the systematic investigation of one's own practice with the goal of improving it (Burns, 2010) — provides an accessible methodology for language teachers integrating AI tools into their classrooms. While action research typically carries less weight than experimental or DBR studies in terms of generalizable knowledge claims, it is valuable for generating practice-based insights and for empowering teachers as researcher-practitioners.

A teacher conducting action research on AI-assisted vocabulary instruction might follow a cycle of planning (selecting an AI vocabulary tool and defining learning objectives), acting (implementing the tool in class over four weeks), observing (collecting data through vocabulary tests, learner surveys, and teaching journal entries), and reflecting (analyzing the data and drawing conclusions to inform the next cycle). The iterative nature of action research aligns well with the rapidly evolving AI landscape, allowing teachers to adapt their practice as both AI tools and their understanding of those tools develop.

For the AI-SLA field, aggregated action research findings — compiled through meta-syntheses or published in practitioner-oriented journals — can provide valuable evidence about how AI tools function in the messy reality of actual classrooms, complementing the controlled findings of laboratory and quasi-experimental studies.

---

## 14.6 Specific Methodological Tools for AI-SLA Research

### 14.6.1 Stimulated Recall for AI Interactions

Stimulated recall (SR) — the technique of replaying a recorded interaction and asking participants to describe their concurrent thoughts (Gass & Mackey, 2000) — is particularly valuable for AI-SLA research because AI interactions are automatically recorded, eliminating the need for external recording equipment and ensuring complete capture of the interaction.

In an AI-SLA stimulated recall study, participants interact with an AI language learning tool while the system logs the entire interaction (text, audio, timestamps, and any other interaction data). Shortly after the interaction — typically within 24 hours to minimize memory decay — participants review the log and narrate their thought processes. "What were you thinking when the AI corrected your sentence here?" "Why did you rephrase your question at this point?" "Did you notice this feedback? What did you do with it?"

The automated logging of AI interactions offers methodological advantages over traditional SR. Researchers can select specific episodes for recall with precision, focusing on moments where the AI provided feedback, where the learner paused for an extended period (possibly indicating cognitive processing), or where the learner produced an unusual utterance. The log also provides an objective record against which the participant's recall can be triangulated — if a participant claims to have noticed an AI correction but the log shows they continued without pausing or revising, this discrepancy is itself informative.

### 14.6.2 Think-Aloud Protocols

Think-aloud protocols, in which participants verbalize their thoughts while performing a task, provide real-time access to cognitive processes that may be lost in retrospective recall. For AI-SLA research, think-aloud data can reveal how learners interpret AI feedback, how they decide whether to accept or reject AI suggestions, and what metalinguistic reasoning they employ when evaluating AI-generated language.

Bowles (2010) noted that think-aloud protocols in SLA research face the challenge of reactivity — the act of verbalizing may alter the cognitive processes being studied. This concern is particularly relevant for AI interaction, because the cognitive demands of simultaneously thinking aloud and formulating target language output may overwhelm learners' processing capacity, producing interaction patterns that differ from naturalistic use. Researchers should consider whether the task complexity (AI interaction plus think-aloud verbalization) is appropriate for participants at a given proficiency level and should report any evidence of reactivity in their findings.

### 14.6.3 Logging and Trace Analysis

AI systems automatically generate detailed logs of learner behavior that can serve as primary or supplementary data sources. These logs typically include timestamped records of every user input, AI response, user interface action (button clicks, navigation, feature use), and sometimes system-internal data (confidence scores, feature weights, decision pathways).

Log analysis can address research questions that are difficult to investigate through other methods. How long do learners spend reviewing AI feedback before moving on? How frequently do they revise their output after receiving corrections? Do they use the AI's grammatical explanations or skip directly to the corrected form? How does their interaction pattern change over time — do they become more or less dependent on AI support? These behavioral questions can be answered at scale through log analysis, providing population-level insights that complement the depth of case study and qualitative approaches.

However, log data must be interpreted with caution. A learner who pauses for thirty seconds after receiving feedback may be deeply processing the correction, or may be checking their phone. A learner who immediately accepts an AI correction may have already known the correct form, or may be unthinkingly clicking through feedback without engagement. Log data reveals what learners do but not why they do it — a limitation that underscores the value of mixed-methods designs combining log analysis with qualitative investigation of learner cognition and motivation.

---

## 14.7 Ethical Considerations in AI Research with Language Learners

### 14.7.1 Informed Consent in AI-Mediated Environments

The ethical principle of informed consent — that research participants should understand what they are agreeing to and participate voluntarily — faces new challenges in AI-SLA research. When a learner interacts with an AI system, the nature of the interaction itself may be difficult to explain to participants in advance. How does one meaningfully inform a participant about the capabilities and limitations of a large language model? How does one explain that the AI may generate incorrect information, exhibit biases, or behave unpredictably — without inducing the very anxiety that undermines ecological validity?

Furthermore, the sheer volume of data collected by AI systems raises questions about what participants are consenting to. A learner who consents to "participating in a study of AI-assisted language learning" may not realize that the AI system will record every keystroke, every pause duration, every revision, and every navigation action — generating a behavioral profile of extraordinary granularity. Consent procedures should explicitly enumerate the types of data collected, the duration of data retention, the parties who will have access, and the measures taken to protect confidentiality.

### 14.7.2 Privacy and Data Protection

AI-SLA research generates data that, in aggregate, can reveal sensitive information about participants: their linguistic proficiency (which may be stigmatized), their educational background, their cognitive processing patterns, and — if the AI interactions involve personal topics — aspects of their personal lives, beliefs, and identities. This data requires protection commensurate with its sensitivity.

Regulatory frameworks such as the General Data Protection Regulation (GDPR) in the European Union and the Family Educational Rights and Privacy Act (FERPA) in the United States impose specific obligations on researchers collecting and processing personal data. AI-SLA researchers must be aware of which regulatory frameworks apply to their studies and must design their data collection, storage, and sharing procedures accordingly.

Practical measures include pseudonymization of all data (replacing identifying information with codes), storage on encrypted, access-controlled systems, strict limitation of data access to authorized research team members, and clear data destruction timelines. When AI interaction data is shared for replication or secondary analysis — a desirable practice for open science — researchers must ensure that shared datasets have been adequately de-identified and that re-identification is not feasible from the data alone or in combination with other available information.

### 14.7.3 Vulnerable Populations

Language learners constitute a population that may be vulnerable in research contexts. Many L2 learners are immigrants, refugees, or international students who may feel pressure to participate in research conducted by their teachers or institutional affiliates. Heritage language learners may belong to marginalized linguistic communities. Young learners lack the capacity for autonomous informed consent. Learners with limited literacy in the research language may not fully understand consent documents.

AI adds additional dimensions of vulnerability. Learners who are not digital natives may be unfamiliar or uncomfortable with AI systems. Learners from cultures where technology use is gendered, restricted, or stigmatized may face social consequences for participating in AI-mediated research. Learners who struggle with the target language may be unable to effectively interact with an AI system that does not support their L1, leading to frustration and potential harm to their language learning motivation.

Researchers must design studies with these vulnerabilities in mind, providing consent materials in participants' strongest language, offering genuine alternatives for those who decline to participate, ensuring that participation does not affect grades or institutional standing, and monitoring for signs of distress or disengagement during AI interactions.

### 14.7.4 AI Bias and Research Ethics

The biases embedded in AI systems — racial, linguistic, gendered, and cultural — create ethical obligations for researchers who deploy these systems with human participants. If an AI pronunciation assessment tool systematically scores speakers of African American Vernacular English (AAVE) lower than speakers of Mainstream American English, deploying this tool in a study with Black participants exposes them to racially biased evaluation. If an AI chatbot responds to code-switched input with "corrections" that devalue the learner's home language variety, the research interaction itself may cause harm to participants' linguistic identity.

Researchers have an ethical obligation to evaluate AI systems for bias before deploying them with participants, to disclose known biases in consent materials and publications, and to include bias analysis as a component of their research design. Studies that uncover AI biases should report them prominently rather than treating them as incidental findings, contributing to the field's collective understanding of how AI systems may harm language learners from marginalized communities.

---

## 14.8 The Replication Crisis and AI Research

### 14.8.1 Replicability Challenges Specific to AI-SLA

The broader scientific replication crisis (Open Science Collaboration, 2015) affects SLA research as it does other fields (Marsden et al., 2018), but AI-SLA research faces additional replication challenges unique to the domain. The moving target problem (Section 14.2.1) means that exact replication of a study conducted on a specific AI system at a specific time point may be literally impossible if the system has since been updated. The personalization paradox (Section 14.2.2) means that even with the same system, different participants will receive different treatments, making exact replication at the individual level impossible.

These challenges do not excuse the field from pursuing replicability; they demand more creative and rigorous approaches to it. Conceptual replication — conducting a new study that tests the same theoretical hypothesis with different participants, different AI systems, or different operationalizations — is often more appropriate and more informative than exact replication in AI-SLA contexts. If the theoretical claim is that AI-generated corrective feedback promotes noticing of morphosyntactic errors, this claim can be tested across different AI systems, different target languages, and different feedback delivery methods. Convergent evidence from multiple conceptual replications provides stronger support than exact replication of a single study.

### 14.8.2 Open Science Practices for AI-SLA Research

Open science practices — pre-registration, open materials, open data, and open analysis code — are particularly important for AI-SLA research given the novelty and rapid evolution of the field. Pre-registration of research hypotheses, methods, and analysis plans on platforms such as OSF (Open Science Framework) or AsPredicted protects against post-hoc hypothesizing and selective reporting, practices to which AI-SLA research may be especially susceptible given the richness of AI interaction data and the temptation to explore multiple outcomes.

Open materials should include, at minimum, the system prompts, configuration parameters, and interaction scripts used to configure AI systems in the study. For studies using commercial APIs, researchers should archive the system's responses to a set of standardized probe inputs at the time of data collection, providing a record of system behavior that can be compared to later versions. For studies using open-source models, sharing the exact model weights and inference code enables exact replication — a level of reproducibility impossible with proprietary systems.

The IRIS database (Instruments for Research into Second Languages, iris-database.org), which archives SLA research materials for sharing and reuse, provides a valuable repository for AI-SLA research instruments, including system prompts, task scripts, assessment rubrics, and analysis protocols.

### 14.8.3 Reporting Standards

The field would benefit from agreed-upon reporting standards for AI-SLA studies, analogous to the CONSORT guidelines for clinical trials or the PRISMA guidelines for systematic reviews. Such standards might require reporting of:

1. **AI system specifications**: Model name and version, API endpoint or software version, system prompt or configuration (full text), temperature and other generation parameters, date(s) of data collection.

2. **Interaction parameters**: Average number of turns per participant, average session duration, total interaction time, any constraints imposed on the interaction.

3. **Data collected**: Complete list of data types collected, with sample sizes for each. Whether AI interaction logs are included as supplementary materials.

4. **Analytical transparency**: Whether analysis was pre-registered, whether any outcomes or covariates were selected post-hoc, sensitivity analyses conducted.

5. **AI behavior validation**: Evidence that the AI system behaved as intended during the study (e.g., analysis of feedback accuracy, response appropriateness, adherence to system prompt instructions).

6. **Effect sizes and confidence intervals**: In addition to p-values, reporting of standardized effect sizes (Cohen's d, eta-squared, or equivalent) and confidence intervals, consistent with best practices in SLA research (Plonsky & Oswald, 2014).

---

## 14.9 A Research Agenda for AI-SLA

### 14.9.1 Theoretical Questions

The preceding chapters of this book have raised numerous theoretical questions that require empirical investigation. The following research agenda, organized by theoretical domain, is offered not as an exhaustive list but as a set of high-priority questions that, if addressed rigorously, would substantially advance the field.

**Input and intake**: Does AI-generated input trigger the same noticing and intake processes as human-generated input? Does the infinite availability of AI-generated input at i+1 level accelerate acquisition, or does the absence of genuine communicative context reduce the efficacy of the input? How does the learner's awareness that input is AI-generated (or their lack of awareness) affect processing?

**Interaction**: Can AI-learner interaction produce the interactional modifications (confirmation checks, clarification requests, comprehension checks, recasts) that Long's Interaction Hypothesis identifies as facilitative of acquisition? If so, are these modifications as effective when they originate from an AI interlocutor as from a human interlocutor? What role does genuine communicative intent play in the acquisition-facilitating properties of interaction?

**Output and feedback**: Does AI scaffolding of output promote or inhibit the three functions Swain identified (noticing, hypothesis testing, metalinguistic reflection)? Under what conditions does AI corrective feedback promote uptake, and how do these conditions compare to findings from the human corrective feedback literature? What is the optimal balance between AI support and productive struggle?

**Identity and motivation**: How does interacting with AI affect learners' investment in the target language community? Does the removal of social risk in AI conversation promote willingness to communicate, or does it deprive learners of the identity-relevant experiences that drive long-term investment? How do learners construct and negotiate their identities as language users in AI-mediated contexts?

**Multilingualism**: How do AI tools support or undermine multilingual repertoire development? Can AI systems be designed to promote translanguaging practices, and do such practices enhance or hinder acquisition of specific target language features? What is the impact of AI on heritage language maintenance?

### 14.9.2 Methodological Priorities

Beyond specific research questions, the field needs methodological development in several areas:

**Longitudinal studies**: The vast majority of existing AI-SLA studies span weeks, not months or years. Longitudinal research tracking learners' engagement with AI tools over extended periods is essential for understanding whether AI produces durable learning gains and how learners' relationship with AI tools evolves over time.

**Multi-tool ecosystem studies**: Research that examines how learners use multiple AI tools in combination, rather than isolating single tools, would better reflect the ecological reality of contemporary language learning.

**Population diversity**: Much existing research is conducted with university students in wealthy countries. Studies involving learners of diverse ages, socioeconomic backgrounds, educational levels, and L1 backgrounds are needed to assess the generalizability of findings.

**Replication and meta-analysis**: As the literature matures, systematic reviews and meta-analyses synthesizing findings across studies will be essential for identifying robust effects, moderating variables, and gaps in the evidence base.

### 14.9.3 Interdisciplinary Collaboration

The complexity of AI-SLA research demands collaboration across disciplinary boundaries. Applied linguists bring theoretical knowledge of language acquisition; computer scientists bring technical understanding of AI systems; psychologists bring expertise in cognition, motivation, and measurement; educational researchers bring methodological traditions for studying learning in complex environments; and sociolinguists bring critical perspectives on language ideology, power, and identity.

No single researcher can possess expertise across all these domains, and no single study can address all dimensions of AI-mediated language learning. The future of the field depends on interdisciplinary research teams that combine complementary expertise, collaborative networks that share instruments, data, and analytical tools, and publication venues that welcome and reward interdisciplinary work.

---

## 14.10 Conclusion: Toward Methodological Maturity

The study of AI in SLA is at a critical juncture. The technology has advanced far beyond the field's capacity to study it — LLMs have been widely adopted for language learning practice before empirical research has established their effects on acquisition, let alone the mechanisms through which those effects operate. This reality creates both urgency and responsibility.

The urgency lies in the need for evidence. Language learners, teachers, and program administrators are making decisions about AI adoption daily, and they deserve evidence-based guidance rather than hype-driven advocacy or fear-driven prohibition. The responsibility lies in the quality of the evidence produced. Poorly designed studies that overstate AI's benefits or understate its risks do more harm than no studies at all, because they provide a false basis for consequential decisions.

This chapter has argued that the methodological toolkit for AI-SLA research already exists in large part — in the experimental, qualitative, and mixed-methods traditions of SLA research, in the learning analytics methods of educational data science, and in the design-based research approaches of educational technology. What is needed is not methodological invention but methodological adaptation, rigor, and ambition: the adaptation of established methods to the unique challenges of AI-mediated environments, the rigor to execute complex designs with adequate samples and appropriate analyses, and the ambition to address the theoretical questions that matter most rather than the technological questions that are easiest to study.

The researchers who will shape this field in the coming decade face an extraordinary opportunity. They stand at the intersection of two of the most dynamic areas of human inquiry — artificial intelligence and second language acquisition — with access to data, tools, and research populations that previous generations of scholars could not have imagined. The methodological foundations described in this chapter are intended to help them seize that opportunity with the rigor it demands and the imagination it deserves.

---

## Discussion Questions

1. Design a study to test whether AI-generated corrective feedback produces comparable learning gains to human tutor feedback for a specific grammatical structure in a specific L2. Specify your research question, participants, treatment and control conditions, measures, and analysis plan. What threats to internal and external validity would you need to address?

2. How would you design a study to investigate the "novelty effect" in AI language learning tools? What design features would allow you to distinguish genuine learning gains from short-term engagement effects?

3. Consider the ethical challenges of conducting research on AI language learning with refugee populations. What special protections would be necessary? How would you balance the potential benefits of AI-assisted language learning with the vulnerabilities of this population?

4. You have access to six months of interaction logs from an AI language tutoring platform used by 5,000 learners. What research questions could you address with this data? What research questions could you NOT address, and what additional data would you need?

5. A colleague argues that pre-registration is unnecessary for AI-SLA research because the field is too new for confirmatory studies — all research should be exploratory. How would you respond?

---

## Practical Applications: Research Design Templates

**Template 1: Quasi-Experimental Pre-Post Design**

| Component | Specification |
|-----------|--------------|
| Research Question | Does AI chatbot conversation practice improve oral fluency more than traditional pair work? |
| Participants | N = 60 intermediate ESL learners, two intact class sections |
| Treatment | 20 minutes of AI chatbot conversation practice, 3x per week, 8 weeks |
| Control | 20 minutes of human pair conversation practice, same topics and frequency |
| Pre-test | ACTFL OPI (or OPIc), timed monologue task (CAF analysis) |
| Post-test | Same measures, parallel forms where available |
| Process data | AI interaction logs, classroom observation notes, learner journals |
| Analysis | ANCOVA with pre-test as covariate; mixed-effects growth model for CAF |
| Ethical safeguards | Crossover after 8 weeks; consent in L1; grade-independent participation |

**Template 2: Mixed-Methods Explanatory Sequential Design**

| Phase | Activity |
|-------|----------|
| Phase 1 (Quantitative) | Pre-registered quasi-experiment comparing AI writing feedback to human feedback (N = 80), measuring writing quality (holistic + analytic rubric), revision behavior (log analysis), and grammatical accuracy (automated + human scoring) |
| Phase 2 (Qualitative) | Stimulated recall interviews with 12 purposefully selected participants (4 high-gain, 4 low-gain, 4 no-gain from each condition), analyzing how learners process and respond to AI vs. human feedback |
| Integration | Qualitative themes mapped onto quantitative outcome patterns to explain why some learners benefit from AI feedback and others do not |

**Template 3: Design-Based Research Cycle**

| Iteration | Focus |
|-----------|-------|
| Iteration 1 | Deploy AI pronunciation tutor prototype; collect interaction logs + user interviews; identify design failures and learning opportunities |
| Iteration 2 | Redesign feedback mechanism based on Iteration 1 findings; test with new cohort; measure pronunciation improvement + learner satisfaction |
| Iteration 3 | Add adaptive difficulty and L1-specific error targeting; longitudinal study (one semester) with mixed-methods evaluation |
| Theory output | Principles for AI pronunciation feedback design grounded in Flege's SLM-r and empirical data from three design cycles |

---

## References

Boot, W. R., Simons, D. J., Stothart, C., & Stutts, C. (2013). The pervasive problem with placebos in psychology: Why active control groups are not sufficient to rule out placebo effects. *Perspectives on Psychological Science*, 8(4), 445-454.

Bowles, M. A. (2010). The think-aloud controversy in second language research. *Routledge*.

Burns, A. (2010). *Doing action research in English language teaching: A guide for practitioners*. Routledge.

Chapelle, C. A. (2001). *Computer applications in second language acquisition*. Cambridge University Press.

Collins, A., Joseph, D., & Bielaczyc, K. (2004). Design research: Theoretical and methodological issues. *The Journal of the Learning Sciences*, 13(1), 15-42.

Craig, P., Dieppe, P., Macintyre, S., Michie, S., Nazareth, I., & Petticrew, M. (2008). Developing and evaluating complex interventions: The new Medical Research Council guidance. *BMJ*, 337, a1655.

Creswell, J. W., & Plano Clark, V. L. (2018). *Designing and conducting mixed methods research* (3rd ed.). SAGE.

Duff, P. A. (2008). *Case study research in applied linguistics*. Lawrence Erlbaum.

Duff, P. A. (2014). Case study research on language learning and use. *Annual Review of Applied Linguistics*, 34, 233-255.

Fairclough, N. (1992). *Discourse and social change*. Polity Press.

Gass, S. M., & Mackey, A. (2000). *Stimulated recall methodology in second language research*. Lawrence Erlbaum.

Gass, S. M., & Mackey, A. (2012). *The Routledge handbook of second language acquisition*. Routledge.

Geertz, C. (1973). *The interpretation of cultures*. Basic Books.

Heritage, J., & Atkinson, J. M. (1984). Introduction. In J. M. Atkinson & J. Heritage (Eds.), *Structures of social action* (pp. 1-15). Cambridge University Press.

Hine, C. (2015). *Ethnography for the internet: Embedded, embodied, and everyday*. Bloomsbury Academic.

Jobin, A., Ienca, M., & Vayena, E. (2019). The global landscape of AI ethics guidelines. *Nature Machine Intelligence*, 1(9), 389-399.

Kress, G., & van Leeuwen, T. (2001). *Multimodal discourse: The modes and media of contemporary communication*. Arnold.

Kyle, K., & Crossley, S. A. (2015). Automatically assessing lexical sophistication: Indices, tools, findings, and application. *TESOL Quarterly*, 49(4), 757-786.

Larsen-Freeman, D., & Cameron, L. (2008). *Complex systems and applied linguistics*. Oxford University Press.

Li, S. (2010). The effectiveness of corrective feedback in SLA: A meta-analysis. *Language Learning*, 60(2), 309-365.

Lu, X. (2010). Automatic analysis of syntactic complexity in second language writing. *International Journal of Corpus Linguistics*, 15(4), 474-496.

Lyster, R., & Ranta, L. (1997). Corrective feedback and learner uptake. *Studies in Second Language Acquisition*, 19(1), 37-66.

Marsden, E., Morgan-Short, K., Thompson, S., & Abugaber, D. (2018). Replication in second language research: Narrative and systematic reviews and recommendations for the field. *Language Learning*, 68(2), 321-391.

Open Science Collaboration. (2015). Estimating the reproducibility of psychological science. *Science*, 349(6251), aac4716.

Pink, S., Horst, H., Postill, J., Hjorth, L., Lewis, T., & Tacchi, J. (2016). *Digital ethnography: Principles and practice*. SAGE.

Plonsky, L. (2013). Study quality in SLA: An assessment of designs, analyses, and reporting practices in quantitative research. *Studies in Second Language Acquisition*, 35(4), 655-687.

Plonsky, L., & Gass, S. (2011). Quantitative research methods, study quality, and outcomes: The case of interaction research. *Language Learning*, 61(2), 325-366.

Plonsky, L., & Oswald, F. L. (2014). How big is "big"? Interpreting effect sizes in L2 research. *Language Learning*, 64(4), 878-912.

Siemens, G., & Baker, R. S. (2012). Learning analytics and educational data mining: Towards communication and collaboration. *Proceedings of the 2nd International Conference on Learning Analytics and Knowledge*, 252-254.

Thorne, S. L. (2003). Artifacts and cultures-of-use in intercultural communication. *Language Learning & Technology*, 7(2), 38-67.

Wong, J., & Waring, H. Z. (2023). Conversation analysis and AI-learner interaction: Preliminary observations on turn-taking and repair. *Applied Linguistics*, 44(3), 456-478.
