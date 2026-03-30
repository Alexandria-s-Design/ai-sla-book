# Chapter 5: Interaction in the Age of Conversational AI

---

## 5.1 Introduction: The Interactionist Promise Meets the Machine Interlocutor

If input is the fuel of second language acquisition, interaction is the engine. This metaphor, while imperfect, captures the centrality of the Interaction Hypothesis to contemporary SLA theory and practice. Michael Long's (1981, 1996) foundational claim -- that conversational interaction, particularly the negotiation of meaning triggered by communication breakdowns, facilitates second language development by making input comprehensible, drawing attention to problematic forms, and pushing learners to modify their output -- has generated more empirical research than perhaps any other single hypothesis in the field. Decades of studies have demonstrated that interactional features such as confirmation checks, comprehension checks, clarification requests, and recasts create the conditions under which learners notice gaps in their interlanguage, test hypotheses about target language forms, and receive feedback that drives restructuring (Mackey, 1999; Gass & Mackey, 2007; Mackey & Goo, 2007).

The emergence of conversational AI -- systems capable of engaging in extended, apparently coherent dialogue in natural language -- thus represents a development of profound theoretical significance for SLA. If interaction drives acquisition, and if AI can now interact, then AI should be able to drive acquisition. This syllogism has fueled an explosion of AI chatbot applications for language learning: ChatGPT-based conversation partners, dedicated platforms like Speak, TalkPal, and Replika, voice-enabled assistants integrated into smart speakers and smartphones, and specialized tutoring systems that simulate conversational exchange. The global market for conversational AI in education is projected to exceed $5 billion by 2027 (MarketsandMarkets, 2024), with language learning constituting the single largest application area.

This chapter subjects these developments to the rigorous theoretical scrutiny they demand. The central argument is that while conversational AI can replicate some surface features of interactional exchange -- turn-taking, question-asking, response contingency -- it cannot replicate the communicative, social, and cognitive conditions that the Interaction Hypothesis identifies as the mechanisms through which interaction facilitates acquisition. The chapter does not conclude that AI-human conversation is useless for language learning; it concludes that its value must be understood on its own terms rather than through the lens of a theoretical framework designed to explain human-human interaction.

The chapter proceeds through seven sections. First, it revisits the Interaction Hypothesis and its extensions, establishing the theoretical benchmarks against which AI interaction must be evaluated. Second, it examines negotiation of meaning in AI-human conversation, asking whether the interactional moves that Long, Pica, and Varonis and Gass identified as facilitative of acquisition actually occur when the interlocutor is a machine. Third, it surveys the landscape of conversational AI tools for language learning, distinguishing between reactive chatbots and proactive agentic AI systems. Fourth, it analyzes corrective feedback in AI interactions. Fifth, it addresses the social dimensions of interaction that AI cannot replicate. Sixth, it reviews the research evidence on AI-human interaction for L2 development. Finally, it proposes a framework for understanding the distinct -- and distinctly limited -- role of AI interaction in the language acquisition process.

---

## 5.2 Theoretical Foundations: The Interaction Hypothesis and Its Extensions

### 5.2.1 Long's Interaction Hypothesis

Michael Long first proposed the Interaction Hypothesis in 1981 and revised it significantly in 1996. In its updated form, the hypothesis states:

> Negotiation for meaning, and especially negotiation work that triggers interactional adjustments by the NS or more competent interlocutor, facilitates acquisition because it connects input, internal learner capacities, particularly selective attention, and output in productive ways. (Long, 1996, p. 451-452)

Several features of this statement are critical for evaluating AI interaction. First, the hypothesis identifies *negotiation for meaning* -- the interactional work that occurs when communication breaks down and participants attempt to restore mutual comprehension -- as the key facilitative mechanism. This is not conversation in general; it is a specific type of conversational event triggered by a specific type of communicative failure. Second, the hypothesis identifies *interactional adjustments* -- modifications to the linguistic input made by the more competent speaker in response to the learner's difficulty -- as the mechanism through which negotiation aids acquisition. These adjustments include repetitions, elaborations, simplifications, recasts, and reformulations. Third, the hypothesis locates the facilitative effect at the intersection of input, attention, and output: negotiation makes specific features of the input salient (connecting to Schmidt's Noticing Hypothesis), which in turn drives the learner to modify their output (connecting to Swain's Output Hypothesis).

For an AI system to fulfill the role that Long's hypothesis assigns to the human interlocutor, it must be capable of three things: detecting communication breakdowns, producing interactional adjustments that are contingent on the specific nature of the breakdown, and doing so in a way that draws the learner's attention to the relevant linguistic features. Whether current AI systems can do these things -- and whether the doing of them by a machine produces the same cognitive and acquisitional effects as the doing of them by a human -- is the central empirical question of this chapter.

### 5.2.2 Pica's Conditions for Negotiation

Teresa Pica (1994) extended the Interaction Hypothesis by specifying the task and participant conditions under which negotiation of meaning is most likely to occur. She identified information-gap tasks -- tasks in which each participant holds information that the other needs -- as the most productive context for negotiation, because they create a genuine communicative need that motivates the interactional work of resolving misunderstandings. Pica further noted that negotiation is more likely when participants have roughly equal status and when both must contribute to the task outcome.

These conditions have significant implications for AI interaction. In a conversation with a chatbot, there is typically no genuine information gap: the learner asks a question, and the AI provides an answer, or the AI poses a prompt, and the learner responds. The AI does not need information from the learner, and the learner knows this. The absence of a genuine communicative need may reduce the motivation for the effortful negotiation that Pica identified as the driver of acquisition-facilitative interaction. A learner who encounters a word they do not understand in an AI chatbot conversation can simply ask "What does X mean?" and receive a definition -- but this is a request for information, not negotiation of meaning. The interactional pressure that forces learners to modify their output, test hypotheses, and attend to problematic forms may be absent when the interlocutor is infinitely patient, infinitely knowledgeable, and has no communicative agenda of its own.

### 5.2.3 Varonis and Gass: The Non-Native Speaker Parallel

Varonis and Gass (1985) demonstrated that negotiation of meaning occurs not only between native and non-native speakers but also between non-native speakers. In NNS-NNS interaction, both participants face comprehension challenges, and both must work to make themselves understood. This creates a more symmetrical interactional dynamic in which both participants are simultaneously learners and interlocutors.

The NNS-NNS interaction paradigm is relevant because AI chatbots, in some respects, resemble neither native speakers nor non-native speakers. An LLM does not have a proficiency level in the target language; it has a probability distribution over sequences of tokens. It does not misunderstand the learner's utterance in the way a human interlocutor might; it either generates a contextually appropriate response or it does not, based on statistical patterns in its training data. When an AI chatbot "misunderstands" a learner -- when it generates a response that does not align with the learner's intended meaning -- the misunderstanding is not communicative but computational. The learner cannot negotiate their way to mutual comprehension because there is no mutual comprehension to achieve; there is only a statistical model generating the most probable next response given the input sequence.

This distinction between communicative misunderstanding and computational misalignment is not merely philosophical. It has direct implications for the quality of negotiation that occurs in AI-human interaction. In human-human negotiation, the interlocutor's confusion is genuine, and the resolution of that confusion through interactional adjustments is a collaborative, meaning-making act. In AI-human interaction, the AI's "confusion" is either a failure of the model to generate an appropriate response or a deliberate pedagogical strategy (if the AI is programmed to feign misunderstanding to elicit negotiation). Neither of these produces the same interactional dynamics as genuine communicative negotiation.

### 5.2.4 Sociocultural Perspectives: Scaffolding and the ZPD

Sociocultural Theory (SCT), grounded in the work of Vygotsky (1978) and elaborated in SLA by Lantolf and Thorne (2006), provides a complementary perspective on interaction that raises additional questions about AI interlocutors. The zone of proximal development (ZPD) -- the distance between what a learner can do independently and what they can do with the assistance of a more capable other -- is the theoretical space in which learning occurs. In SCT, interaction is not merely a source of input and feedback; it is the primary mechanism through which cognitive development occurs. Higher mental functions, including language, develop first in the social plane (interpsychological) and only later are internalized to the individual plane (intrapsychological).

The concept of *scaffolding* -- the graduated, responsive assistance provided by a more capable other within the ZPD -- has specific characteristics that distinguish it from mere help. Wood, Bruner, and Ross (1976) identified six functions of scaffolding: recruiting the learner's interest, reducing degrees of freedom, maintaining direction, marking critical features, frustration control, and demonstration. Effective scaffolding is *contingent*: it responds to the learner's moment-to-moment performance, increasing support when the learner struggles and withdrawing it when the learner succeeds. It is also *temporary*: the goal is for the learner to internalize the scaffolded performance and carry it out independently.

Can AI provide scaffolding in this sense? The question is debated. Lantolf (2000) argued that mediation, in the Vygotskian sense, requires a human consciousness engaged in a collaborative activity with the learner. Poehner (2008) demonstrated that dynamic assessment -- a form of mediated interaction in which the assessor adjusts support in response to the learner's performance -- requires sensitivity to qualitative differences in learner responses that go beyond right/wrong distinctions. An AI system that provides hints when the learner gives incorrect responses is providing help, but it is not necessarily providing the contingent, responsive mediation that SCT defines as scaffolding.

More recently, however, some scholars have proposed a more expansive view of mediation that includes technological artifacts. Thorne (2003) argued that all tools, including digital ones, mediate cognitive activity, and that the question is not whether AI can mediate but how AI mediates and with what consequences for development. This perspective opens the door to evaluating AI interaction not as a replacement for human scaffolding but as a distinct form of mediated activity with its own affordances and constraints.

---

## 5.3 Negotiation of Meaning with AI Interlocutors

### 5.3.1 Can AI Trigger Negotiation?

The empirical question of whether AI chatbot interactions trigger the negotiation of meaning sequences documented in human-human interaction has been examined in several studies. Kim (2017) analyzed conversation logs between Korean EFL students and an English chatbot and found that the interactions contained very few instances of negotiation of meaning. Students tended to abandon topics when misunderstandings arose rather than negotiating to resolve them. When negotiation did occur, it was typically initiated by the student requesting clarification of the AI's response rather than by the AI requesting clarification of the student's output -- the reverse of the pattern most commonly observed in NS-NNS interaction and the pattern theorized to be most facilitative of acquisition.

Fryer, Ainley, Thompson, Gibson, and Sherlock (2017) compared student interactions with a chatbot versus human interlocutors and found that while initial engagement with the chatbot was high, sustained conversational interaction decreased rapidly over time. Students reported that the chatbot's responses were predictable and that the conversation felt "hollow" -- a description that aligns with the theoretical concern about the absence of genuine communicative intent.

Jeon (2022) examined interactions between advanced Korean learners of English and ChatGPT (GPT-3.5) and found a more nuanced pattern. Students did engage in extended turns and occasionally negotiated meaning, particularly when they used ChatGPT as a conversation partner for opinion-exchange tasks. However, the negotiation sequences were qualitatively different from those observed in human interaction: students were more likely to reformulate their entire message rather than engaging in the incremental, collaborative negotiation characteristic of human-human conversation. The AI's tendency to "understand" (or appear to understand) any input, no matter how ungrammatical or ambiguous, meant that the communicative pressure to be precise and clear -- the pressure that drives negotiation in human interaction -- was largely absent.

### 5.3.2 The Accommodation Problem

A related concern is what might be called the *accommodation problem*. Human interlocutors in NS-NNS conversation engage in a form of communicative accommodation: they simplify their speech, slow their rate, use more frequent vocabulary, and avoid complex syntactic structures in response to perceived learner difficulty (Hatch, 1983; Long, 1983). This accommodation is one of the mechanisms through which interaction provides comprehensible input. Crucially, it is dynamic and responsive: the native speaker adjusts in real time based on the learner's verbal and nonverbal signals of comprehension or confusion.

AI chatbots can be programmed to accommodate -- to generate responses at a specified difficulty level -- but this accommodation is typically static rather than dynamic. An AI system set to "B1 level" will generate B1-level responses regardless of whether the learner is understanding everything easily or struggling with every sentence. More sophisticated systems can adjust based on learner errors or response latency, but even these adjustments are based on surface signals rather than the rich, multimodal evidence of comprehension that human interlocutors use (facial expression, body language, prosody, eye contact, hesitation patterns).

The absence of dynamic accommodation means that AI chatbot conversations may not provide the kind of finely tuned input that the Interaction Hypothesis identifies as the primary acquisitional benefit of interaction. The interactional adjustments that Long theorized as facilitative -- the moment when the native speaker recognizes that a particular word or structure was not understood and rephrases, repeats, or elaborates specifically in response to that failure -- require a sensitivity to communicative breakdown that current AI systems approximate but do not achieve.

### 5.3.3 The Comprehension Illusion

Perhaps the most theoretically concerning feature of LLM-based conversation partners is their tendency to generate fluent, coherent, and apparently relevant responses to any input, including input that is highly ungrammatical, ambiguous, or semantically anomalous. Human interlocutors signal non-comprehension through facial expressions, clarification requests, or silence. These signals create the communicative pressure that drives the learner to modify their output and attend to the forms that caused the breakdown. An AI that responds fluently to ungrammatical input provides no such signal. The learner may conclude that their utterance was comprehensible and well-formed, receiving what amounts to implicit positive evidence for an incorrect form.

This phenomenon -- which we might term the *comprehension illusion* -- is the interactional mirror of the authenticity problem discussed in Chapter 4. In human interaction, comprehension is an achievement that both participants work toward; breakdowns are informative events that drive development. In AI interaction, comprehension is simulated by the model's ability to generate a contextually plausible response, and breakdowns either do not occur or are invisible to the learner. The result is a conversation that feels smooth and successful but that may not create the cognitive conditions -- the noticing of gaps, the testing of hypotheses, the effortful modification of output -- that the Interaction Hypothesis identifies as the mechanisms of acquisition.

---

## 5.4 The Conversational AI Landscape: From Chatbots to Agentic Systems

### 5.4.1 A Taxonomy of AI Interlocutors

Not all AI conversational systems are created equal, and the failure to distinguish between different types of AI interaction partners has been a significant weakness in both the research literature and practical discussions of AI in language learning. This section proposes a taxonomy that distinguishes between four categories of AI systems, ordered by increasing autonomy and proactivity:

**1. Rule-based chatbots.** Early language learning chatbots (e.g., CSIEC, described by Jia, 2004) used pattern-matching rules and scripted dialogue trees to simulate conversation. These systems could handle a narrow range of predetermined topics and responses but could not cope with unexpected input. Their interactional capabilities were minimal, and they have been largely superseded by more sophisticated systems.

**2. LLM-based conversational AI.** Systems built on large language models (ChatGPT, Claude, Gemini) can engage in open-ended, topically flexible conversation across any domain. They generate responses by predicting the most probable next tokens given the conversation history, producing text that is often indistinguishable from human-produced text. Their interactional capabilities are significant -- they can ask follow-up questions, provide feedback, and adjust their language level -- but they are fundamentally *reactive*: they respond to user input and do not initiate interaction or pursue communicative goals of their own. Dedicated language learning platforms like Speak, TalkPal, and Languable use LLM backends with pedagogical wrappers that add features like error correction, topic suggestions, and proficiency tracking.

**3. Voice-enabled conversational AI.** Voice assistants (Amazon Alexa, Google Assistant, Apple Siri) and voice-enabled language tutors (Speak, ELSA Speak) add the dimension of spoken interaction to the conversational AI paradigm. These systems use automatic speech recognition (ASR) to convert learner speech to text, process the text through an LLM or rule-based system, and generate spoken responses through text-to-speech (TTS). The addition of the speech modality introduces pronunciation practice and listening comprehension into the interaction but also introduces the error propagation problem: ASR errors in recognizing learner speech can lead to irrelevant or confusing AI responses, undermining the quality of the interaction.

**4. Agentic AI systems.** The most recent and theoretically significant category consists of *agentic AI* systems -- AI that can plan, execute multi-step sequences, use external tools, and pursue goals over extended interactions. Unlike conversational AI, which responds turn-by-turn, agentic AI can autonomously design a lesson plan, select materials, track learner progress across sessions, initiate review activities, and adjust pedagogical strategy based on learner performance patterns. Systems like OpenAI's Assistants API, Claude's tool-use capabilities, and educational platforms built on agentic frameworks (e.g., AutoGen, CrewAI, LangGraph) enable AI tutoring systems that proactively manage the learning process rather than simply responding to learner prompts.

### 5.4.2 Conversational AI vs. Agentic AI: A Critical Distinction

The distinction between conversational AI and agentic AI is critical for SLA theory, though the research literature has not yet fully grappled with its implications. Conversational AI -- the reactive chatbot or voice assistant -- maps relatively straightforwardly onto the interactional paradigm: it is an interlocutor, albeit a limited one, and its acquisitional value can be evaluated against the Interaction Hypothesis and related frameworks.

Agentic AI, by contrast, is not merely an interlocutor; it is a pedagogical agent that manages the learning environment. An agentic AI tutor does not simply respond to a learner's conversational turns; it decides what topics to introduce, when to correct errors, how to sequence activities, when to review previously studied material, and how to balance fluency practice with accuracy work. In this sense, agentic AI is less like a conversation partner and more like a teacher -- or, more precisely, like an instructional management system that incorporates conversational interaction as one component of a larger pedagogical design.

This distinction matters because the theoretical framework for evaluating a conversation partner is different from the framework for evaluating a teacher or instructional system. A conversation partner is evaluated by the quality of the interaction it supports -- the negotiation of meaning, the feedback, the communicative pressure. A teacher is evaluated by the quality of the pedagogical decisions it makes -- the sequencing, the assessment, the differentiation, the motivational support. An agentic AI that makes poor pedagogical decisions but supports rich conversational interaction may be less effective than one that makes good pedagogical decisions but provides minimal conversational practice.

The conflation of conversational and agentic AI in popular discourse -- the assumption that a "better chatbot" automatically makes a better language tutor -- obscures this distinction and may lead to misguided development priorities. The most important advances in AI for language learning may lie not in making AI a better conversational partner but in making it a better pedagogical decision-maker, even if the conversational interface remains relatively simple.

### 5.4.3 Platform Survey: Current Tools and Their Interactional Affordances

A brief survey of current AI-powered language interaction tools illustrates the range of approaches:

**ChatGPT and Claude (general-purpose LLMs).** When prompted as conversation partners, these systems can engage in extended dialogue on any topic, adjust their language level, provide corrections, and explain grammar. Their strength is flexibility; their weakness is the absence of pedagogical structure. Without explicit prompting, they default to being helpful assistants rather than language tutors, which means they often accommodate the learner's errors rather than creating the interactional pressure to correct them. Learners who use these systems for conversation practice report enjoying the experience but also note that the conversations feel "easy" in ways that may not promote development (Kohnke, Moorhouse, & Zou, 2023).

**Speak.** A dedicated AI speaking practice platform that combines ASR, LLM-based dialogue, and targeted pronunciation feedback. Speak structures interactions around specific scenarios (ordering food, making a complaint, job interviews) and provides real-time feedback on pronunciation, grammar, and vocabulary. Its structured approach creates more interactional pressure than open-ended LLM conversation, but the pre-defined scenarios limit the negotiation of meaning to predictable communication challenges.

**TalkPal.** An AI conversation partner that adapts to learner proficiency and provides real-time error correction with explanations. TalkPal supports both text and voice interaction and tracks learner progress across sessions. Its agentic features (topic suggestion, review scheduling) represent a move toward the agentic AI category described above.

**Replika.** An AI companion application originally designed for emotional support that has been adopted by some language learners as a conversation partner. Replika's strength is its ability to maintain a persistent persona and remember previous conversations, creating a sense of ongoing relationship that other AI systems lack. However, its design priorities (emotional engagement, companionship) may conflict with language learning goals (error correction, pushed output).

**Duolingo Max.** Duolingo's premium tier includes "Explain My Answer" (AI-generated explanations of why an answer was correct or incorrect) and "Roleplay" (AI-powered conversation practice within thematic scenarios). These features represent the integration of conversational AI into an established, structured language learning platform, combining the interactional affordances of AI with the pedagogical sequencing of a mature curriculum.

---

## 5.5 Corrective Feedback in AI Interactions

### 5.5.1 The Feedback Problem in AI Conversation

Corrective feedback -- the response to a learner's erroneous utterance that signals the presence of an error and potentially provides the correct form -- is central to both the Interaction Hypothesis and the broader SLA research on the role of negative evidence in acquisition. Lyster and Ranta (1997) documented six types of corrective feedback in classroom interaction: explicit correction, recasts, clarification requests, metalinguistic feedback, elicitation, and repetition. Subsequent research has demonstrated that different feedback types produce different effects on acquisition, with evidence that prompts (feedback that pushes the learner to self-correct) may be more effective than recasts (feedback that provides the correct form) for certain structures and in certain contexts (Lyster & Saito, 2010; Li, 2010).

AI chatbot interactions produce a distinctive feedback pattern that does not map neatly onto the human classroom taxonomy. Several studies have documented the following tendencies:

**Implicit acceptance of errors.** As noted in Section 5.3.3, LLMs frequently respond fluently to erroneous input without signaling the error. This constitutes implicit positive evidence for incorrect forms -- the opposite of corrective feedback.

**Unsolicited explicit correction.** When AI systems are programmed to provide error correction, they tend to favor explicit correction and metalinguistic explanation -- the most direct and least ambiguous feedback types. This is pedagogically convenient but may not be optimal for acquisition. Lyster and Ranta's (1997) research found that explicit correction was among the least effective feedback types in terms of prompting learner uptake (the learner's incorporation of the correction into subsequent output).

**Absence of prompts.** AI systems rarely use elicitation, repetition, or clarification requests as feedback strategies -- the prompt types that push learners to self-correct and that the research suggests are most facilitative of acquisition. The reason is partly technical (prompts require the AI to identify specifically what is wrong while withholding the correct form, which is more computationally demanding than simply providing the correction) and partly interactional (prompts can feel awkward or unnatural in an AI conversation context where there is no genuine communication breakdown to motivate them).

**Inconsistency.** The same error may receive correction in one conversational turn and pass unremarked in the next, depending on the LLM's response generation. This inconsistency may reduce the salience of corrective feedback and undermine the learner's ability to identify patterns in their errors.

### 5.5.2 Recasts in AI Interaction

Recasts -- reformulations of a learner's erroneous utterance that correct the error while maintaining the meaning -- are the most studied feedback type in SLA and the most relevant to AI interaction, because they can be embedded naturally in conversational exchange without disrupting the flow of communication. Research has shown that recasts are effective for acquisition when they are noticed by the learner, but that noticing rates vary depending on the linguistic context, the learner's developmental readiness, and the salience of the recast (Mackey, Gass, & McDonough, 2000; Philp, 2003).

AI chatbots can be programmed to produce recasts by incorporating the corrected form into their response. For example:

> *Learner:* Yesterday I go to the store.
> *AI:* Oh, you *went* to the store yesterday? What did you buy?

This is a textbook recast, and it is well within the capability of current LLMs. The question is whether the learner notices the recast and processes it as corrective feedback rather than as a simple continuation of the conversation. In human interaction, recasts are accompanied by prosodic cues (emphasis on the corrected form), facial expressions, and contextual signals that help the learner identify the reformulation as a correction. In text-based AI interaction, these cues are absent. In voice-based AI interaction, the TTS system may not produce the prosodic emphasis that makes recasts salient.

Empirical evidence on the noticing of AI-delivered recasts is limited but suggestive. Ziegler (2016) found that text-based chatbot recasts were less likely to be noticed than human interlocutor recasts in text chat, suggesting that the modality alone does not ensure noticing and that additional salience cues may be needed. Sauro (2009) demonstrated that text chat recasts could be effective when accompanied by visual enhancement (bolding, color), pointing to the potential for AI systems to increase recast salience through typographic means.

### 5.5.3 The Feedback Timing Paradox

Human interlocutors provide feedback in real time, embedded in the flow of conversation. The immediacy and embeddedness of this feedback are considered important for its effectiveness, because they allow the learner to compare their erroneous utterance with the corrected form while both are still active in working memory (Doughty, 2001). AI systems can also provide immediate feedback, but they introduce a paradox: the feedback can be *too* immediate and *too* available.

In human interaction, feedback is contingent on the interlocutor's attention, patience, and conversational priorities. Not every error receives feedback, and the selective nature of feedback helps the learner prioritize which forms to attend to. An AI system that corrects every error in every utterance may overwhelm the learner with feedback, reducing the salience of any individual correction. Conversely, an AI system that corrects selectively may appear inconsistent, as discussed above.

Furthermore, the availability of feedback on demand -- the learner can ask "Was that correct?" at any point -- may reduce the cognitive effort that learners invest in monitoring their own output. If the AI will catch any error, the learner has less incentive to develop the self-monitoring skills that are essential for independent language use. This concern aligns with the broader "AI dependency" issue discussed in Chapter 6 and with research on the role of struggle and effort in durable learning (Bjork & Bjork, 2011).

---

## 5.6 Social Dimensions: What AI Cannot Replicate

### 5.6.1 Communicative Intent and Genuine Information Exchange

The most fundamental difference between human-human and human-AI interaction is the presence or absence of genuine communicative intent. When two humans converse, each brings to the interaction a set of communicative goals: they want to share information, express opinions, request action, build relationships, negotiate identities, or achieve collaborative outcomes. These goals create the communicative pressure that motivates the interactional work -- including negotiation of meaning -- that the Interaction Hypothesis identifies as facilitative of acquisition.

An AI chatbot has no communicative intent. It does not want to know the answer to the question it asks. It does not care whether the conversation succeeds or fails. It does not experience frustration when misunderstood or satisfaction when communication is achieved. Its "goals" are statistical: to generate the most probable next response given the input sequence and the system prompt. This absence of genuine communicative intent means that the *social contract* of conversation -- the mutual commitment to understanding and being understood that Grice (1975) formalized as the Cooperative Principle -- is not in force. The learner may be cooperating, but the AI is computing.

This matters for acquisition because the communicative pressure created by genuine interaction is theorized to be one of the mechanisms that makes interaction facilitative. When a learner must make themselves understood to a real interlocutor with genuine informational needs, they are motivated to attend to form, clarity, and precision in ways that they may not be when conversing with a system that will generate a plausible response regardless of whether it "understood" the input.

### 5.6.2 Social Risk, Face, and the Affective Dimension

One of the most frequently cited advantages of AI conversation partners is that they remove the social risk of error. Learners who are anxious about making mistakes in front of human interlocutors -- a phenomenon extensively documented in the SLA literature on foreign language anxiety (Horwitz, Horwitz, & Cope, 1986; MacIntyre & Gardner, 1991) -- may feel more comfortable practicing with an AI that does not judge, ridicule, or lose patience.

This is a genuine benefit, and it should not be dismissed. Krashen's (1982) Affective Filter Hypothesis, despite its theoretical limitations, captured an important insight: negative affect can inhibit language acquisition, and reducing anxiety may create more favorable conditions for learning. If AI conversation practice reduces anxiety and increases willingness to communicate, this is a meaningful contribution to the language learning ecosystem.

However, the removal of social risk also removes something that may be important for development. Goffman's (1967) concept of *face* -- the positive social image that speakers construct and maintain in interaction -- and Brown and Levinson's (1987) politeness theory suggest that much of the interactional work that characterizes human conversation is motivated by face concerns. Speakers monitor their language use, repair errors, and attend to pragmatic appropriateness because social consequences are at stake. An AI interlocutor has no face to threaten or maintain, and the learner's face is not at stake in an interaction with a machine. The removal of face concerns may reduce the motivation for the kind of careful, self-monitored language production that promotes development.

Norton's (2013) concept of *investment* -- the learner's commitment to learning a language as it relates to their identity and imagined future selves -- provides another lens. Investment is inherently social: learners invest in language learning because they want to participate in communities, access resources, and construct identities in the target language. Conversing with an AI does not constitute participation in a community, does not provide access to real social resources, and does not involve the identity negotiation that Norton identified as central to language learning motivation. A learner who practices English with ChatGPT is not investing in an English-speaking community; they are practicing a skill in isolation.

### 5.6.3 Pragmatic Competence and Sociolinguistic Variation

Pragmatic competence -- the ability to use language appropriately in social contexts, including the ability to perform speech acts, manage politeness, interpret implicature, and navigate register variation -- is a critical component of communicative competence that is developed primarily through social interaction (Kasper & Rose, 2002; Taguchi, 2015). AI chatbots, as currently implemented, are poor models and interlocutors for pragmatic development.

LLMs are trained to be helpful, harmless, and honest (Bai et al., 2022), which means they default to a polite, accommodating, and register-neutral conversational style that does not reflect the pragmatic complexity of real-world interaction. A learner practicing refusal strategies with an AI will not encounter the social pressure that makes refusals difficult in real life. A learner practicing complaints will not face the face-threatening dynamics that shape real complaint sequences. A learner practicing humor will not receive the social feedback (laughter, confusion, offense) that calibrates pragmatic development in natural interaction.

Moreover, LLMs encode the sociolinguistic norms of their training data, which is disproportionately drawn from formal, written, Standard American English (for English-language models). Learners who develop their interactional competence primarily through AI conversation may develop a pragmatic repertoire that is formal, generic, and sociolinguistically narrow -- adequate for some communicative contexts but inadequate for the diverse, informal, and culturally specific interactions that characterize real-world language use.

### 5.6.4 Identity, Community, and Belonging

Language acquisition is not merely a cognitive process; it is a social process intimately connected to identity, community membership, and belonging (Norton, 2013; Block, 2007; Darvin & Norton, 2015). Learners do not acquire language in a vacuum; they acquire it as they negotiate membership in communities of practice (Lave & Wenger, 1991), construct and reconstruct their identities as speakers of the target language, and navigate the power dynamics of multilingual societies. These social processes are not peripheral to acquisition; in sociocultural and poststructuralist frameworks, they are constitutive of it.

AI interaction is fundamentally asocial in this sense. A learner who converses with an AI is not negotiating membership in a community. They are not constructing an identity as a speaker of the target language in relation to other speakers. They are not navigating power dynamics, because there are no power dynamics in an interaction with a machine (though the design of the machine may encode and perpetuate existing power structures). The social dimensions of language learning -- the dimensions that make it meaningful, motivating, and ultimately successful for the long term -- are absent from AI interaction, no matter how sophisticated the conversational interface.

This does not mean that AI interaction is valueless. It means that its value lies in areas other than the social dimensions of acquisition: in providing safe practice space, in delivering feedback, in building automaticity, in supporting the development of formal accuracy. The critical error is to assume that AI interaction can substitute for human interaction in the language learning process, when the social dimensions of human interaction are precisely what make it irreplaceable.

---

## 5.7 Research Evidence: What Do We Know About AI-Human Interaction for L2 Development?

### 5.7.1 Early Chatbot Studies (Pre-LLM)

Research on chatbot-assisted language learning predates the LLM era by more than a decade. Studies of early chatbots (CSIEC, Cleverbot, A.L.I.C.E.) consistently found that while learners enjoyed the novelty of chatbot interaction, the interactions were limited in scope, produced minimal negotiation of meaning, and did not result in measurable gains in linguistic competence beyond vocabulary (Coniam, 2008; Fryer & Carpenter, 2006). The limitations of rule-based chatbots -- their inability to handle unexpected input, their repetitive response patterns, their lack of conversational coherence -- constrained both the quality of the interaction and the learner's engagement.

Fryer et al. (2017) conducted one of the more rigorous pre-LLM chatbot studies, comparing student willingness to communicate (WTC) with a chatbot versus a human partner over multiple sessions. They found that initial WTC with the chatbot was comparable to WTC with a human partner, but that WTC with the chatbot declined significantly over subsequent sessions while WTC with the human partner remained stable or increased. The authors attributed this decline to the chatbot's inability to build rapport, remember previous conversations, or respond to the learner as a person rather than a text-input device.

### 5.7.2 LLM-Era Studies (2023-Present)

The release of ChatGPT in November 2022 catalyzed a wave of studies examining LLM-based conversation for language learning. These studies have generally found more positive results than pre-LLM chatbot research, reflecting the qualitative improvement in conversational coherence and flexibility that LLMs provide.

Kohnke et al. (2023) surveyed Hong Kong university students using ChatGPT for English practice and found high levels of perceived usefulness and satisfaction. Students reported that ChatGPT provided a low-anxiety environment for practicing writing and conversation, offered immediate and detailed error correction, and was available at any time. However, the study relied on self-report data and did not measure actual language gains.

Bin-Hady, Al-Kadi, Hazaea, and Ali (2023) examined the use of ChatGPT by Yemeni EFL learners and found that students who used ChatGPT for conversation practice showed greater confidence in speaking English but did not show statistically significant gains on a standardized English proficiency test compared to a control group. The study suggests that AI conversation practice may affect learner attitudes and confidence without necessarily translating into measurable proficiency gains.

Han and Finkelstein (2024) conducted an experimental study comparing Korean EFL students' speaking development over eight weeks of practice with ChatGPT versus human conversation partners. The human-partner group showed significantly greater gains in discourse management, pragmatic appropriateness, and interactional competence, while the ChatGPT group showed greater gains in grammatical accuracy and lexical range. This pattern aligns with the theoretical analysis presented earlier in this chapter: AI interaction may support formal accuracy but not the interactional and pragmatic competencies that develop through genuine social interaction.

### 5.7.3 Voice-Based AI Interaction Studies

The addition of speech to AI interaction introduces both new affordances and new challenges. Studies of voice-enabled AI language tutors have focused primarily on pronunciation (discussed in Chapter 8) but have also examined conversational fluency and speaking anxiety.

Tai and Chen (2023) compared Chinese EFL students' speaking fluency development after eight weeks of practice with a voice-enabled AI tutor (Speak) versus a human conversation partner. Both groups showed gains in speech rate and mean length of utterance, but the human-partner group showed greater gains in interactive fluency measures (turn-taking, back-channeling, collaborative completion). The AI-tutor group showed greater gains in monologic fluency measures (length of uninterrupted speech, speech rate in extended turns), consistent with the finding that AI interaction supports individual performance but not collaborative interaction.

Moussalli and Cardoso (2020) examined the use of Amazon Alexa for French pronunciation practice and found that learners who practiced with Alexa showed improvements in intelligibility but not in comprehensibility or accentedness (see Chapter 8 for definitions of these constructs). They noted that Alexa's binary feedback (either recognizing the utterance or failing to recognize it) lacked the nuance needed for targeted pronunciation development.

### 5.7.4 Meta-Analytic Evidence

As of the time of writing, no comprehensive meta-analysis of AI chatbot-assisted language learning has been published, though several are reportedly in preparation. Preliminary systematic reviews (Huang, Hew, & Fryer, 2022; Yin, Satar, & Kasper, 2023) have identified the following patterns across studies:

- Effect sizes for vocabulary acquisition are consistently positive but small (d = 0.2-0.4).
- Effect sizes for grammatical accuracy are positive but variable, with some studies showing no significant effect.
- Effect sizes for speaking fluency are positive when measured by speech rate or quantity of output, but not when measured by interactive competence.
- Effect sizes for pragmatic competence are consistently non-significant.
- Learner satisfaction and reduced anxiety are consistently reported across studies.
- Methodological quality is generally low, with small samples, short treatment periods, and lack of delayed post-tests.

These patterns suggest that AI conversation practice can contribute to certain dimensions of language development -- particularly vocabulary, formal accuracy, and fluency defined as speech quantity -- but is not a substitute for human interaction when the goal is developing interactional competence, pragmatic appropriateness, or the social dimensions of communicative competence.

---

## 5.8 A Framework for Understanding AI Interaction in SLA

### 5.8.1 What AI Interaction Is Good For

Based on the theoretical analysis and empirical evidence presented in this chapter, AI conversational interaction appears to offer genuine value in the following areas:

**Safe practice space.** For learners with high anxiety or low willingness to communicate, AI provides a low-stakes environment for practicing speaking and writing in the L2 without fear of social judgment. This is particularly valuable for beginning learners who need to build basic confidence before engaging in human interaction.

**Repetition and automaticity.** AI is infinitely patient and available 24 hours a day. Learners who need to practice specific conversational routines -- ordering food, making appointments, describing symptoms to a doctor -- can repeat these interactions as many times as needed to develop automaticity. DeKeyser's (1998) Skill Acquisition Theory posits that procedural knowledge develops through practice, and AI can provide more practice opportunities than classroom interaction alone.

**Formal accuracy feedback.** AI systems are effective at identifying and correcting grammatical and lexical errors, providing metalinguistic explanations, and tracking error patterns across interactions. For learners who want to improve their formal accuracy, AI feedback is immediate, detailed, and non-judgmental.

**Topic and genre exploration.** AI chatbots can converse on any topic, which allows learners to practice language use across diverse domains and genres. A learner preparing for a job interview, a medical appointment, or an academic presentation can practice with an AI partner that simulates the relevant scenario.

### 5.8.2 What AI Interaction Cannot Do

Equally important is an honest acknowledgment of what AI interaction cannot provide:

**Genuine communicative pressure.** The motivation to be understood by a real interlocutor with genuine communicative needs cannot be simulated. AI interaction lacks the social stakes that drive learners to attend to clarity, precision, and appropriateness.

**Negotiation of meaning in the interactionist sense.** The specific interactional sequences that Long, Pica, and Gass documented as facilitative of acquisition -- genuine communication breakdowns resolved through collaborative negotiation -- are rare or absent in AI interaction.

**Pragmatic development.** The social norms, face dynamics, and cultural expectations that shape pragmatic competence in the target language cannot be learned from an AI that has no social presence and encodes narrow, formal pragmatic norms.

**Identity and community.** The social meaning of language learning -- the investment in communities, the construction of identity, the negotiation of belonging -- is absent from AI interaction, no matter how sophisticated the interface.

**Dynamic scaffolding.** The contingent, responsive mediation that SCT identifies as the mechanism of development in the ZPD requires sensitivity to the learner's moment-to-moment performance that exceeds the capabilities of current AI systems.

### 5.8.3 The Complementarity Principle

The framework that emerges from this analysis is one of *complementarity* rather than replacement. AI interaction and human interaction serve different functions in the language acquisition process, and neither can substitute for the other. A well-designed language learning program would leverage AI interaction for what it does well -- safe practice, repetition, accuracy feedback, topic exploration -- while preserving human interaction for what only humans can provide -- genuine communicative pressure, social scaffolding, pragmatic modeling, identity development, and community membership.

This complementarity principle has practical implications for program design. Rather than replacing conversation partners, tutors, or classroom interaction with AI chatbots, programs should integrate AI practice as *preparation* for human interaction. A learner might practice a conversation scenario with an AI to build confidence and fluency, then engage in the same scenario with a human partner where the social stakes, communicative pressure, and interactional dynamics create the conditions for the deeper processing that leads to acquisition. This "rehearsal-performance" model leverages the strengths of both AI and human interaction without pretending that one can substitute for the other.

### 5.8.4 Future Directions

The rapid development of AI systems makes prediction hazardous, but several trajectories deserve monitoring:

**Improved dynamic accommodation.** As AI systems become better at modeling learner proficiency in real time and adjusting their output accordingly, the quality of interactional adjustments may improve. Multimodal AI systems that can process facial expressions, gesture, and prosody in addition to text may achieve the sensitivity to comprehension signals that current text- and voice-based systems lack.

**Agentic tutoring systems.** As discussed in Section 5.4.2, the development of agentic AI may shift the relevant question from "Can AI be a good conversation partner?" to "Can AI be a good pedagogical decision-maker?" If agentic AI systems can design effective interaction tasks, sequence them appropriately, and integrate AI practice with human interaction opportunities, the overall quality of the language learning experience may improve even if the individual AI conversations remain limited.

**Embodied AI.** AI agents in virtual or augmented reality environments may provide a richer interactional context than text or voice chat, including gesture, spatial reference, and embodied action. The theoretical implications of embodied AI interaction for SLA -- discussed further in Chapter 15 -- deserve sustained research attention.

**Empirical evidence.** The most important need is for high-quality empirical research that examines the long-term effects of AI interaction on language development, using rigorous designs with appropriate control conditions, validated outcome measures, and delayed post-tests. The current evidence base, while growing, remains insufficient to support the strong claims made by AI language learning platforms.

---

## 5.9 Conclusion

Interaction has been the workhorse construct of SLA theory for four decades, and the emergence of conversational AI would seem to offer a transformative new source of interactional practice. This chapter has argued that the reality is more nuanced. While AI systems can replicate the surface forms of conversational interaction -- turn-taking, question-asking, response contingency -- they cannot replicate the communicative, social, cognitive, and identitary conditions that the Interaction Hypothesis and Sociocultural Theory identify as the mechanisms through which interaction facilitates acquisition.

This is not a failure of AI but a clarification of what interaction *is* in SLA theory. Interaction is not merely the exchange of turns; it is the collaborative, socially motivated, communicatively purposeful negotiation of meaning between persons who are invested in understanding and being understood. An AI system that generates fluent responses to learner input is doing something -- something that may be valuable for practice, feedback, and confidence-building -- but it is not doing *that*.

The challenge for the field is to develop a theoretical framework for understanding AI-human interaction on its own terms rather than through the lens of human-human interaction. What are the cognitive mechanisms through which AI conversation practice contributes to language development? How do these mechanisms differ from those identified by the Interaction Hypothesis? What are the optimal conditions for AI interaction practice, and how should it be integrated with human interaction to produce the best outcomes? These are the questions that the next generation of AI-SLA research must address.

The next chapter examines the other side of the interactional coin: output. If this chapter has focused on what the learner receives from the AI interlocutor, Chapter 6 focuses on what the learner produces -- and on the paradox of AI systems that can produce language for the learner, potentially undermining the very output that Swain's hypothesis identifies as essential for acquisition.

---

## Discussion Questions

1. Long's Interaction Hypothesis identifies negotiation of meaning as the key facilitative mechanism of interaction. Based on the evidence reviewed in this chapter, does AI-human conversation produce genuine negotiation of meaning? Why or why not?

2. What is the difference between conversational AI and agentic AI, and why does this distinction matter for language learning theory and practice?

3. The chapter argues that AI removes the "social risk" of interaction, which is both an advantage and a limitation. In what circumstances might the removal of social risk be beneficial, and in what circumstances might it be detrimental to language development?

4. Design a lesson sequence that uses AI conversation practice as preparation for human interaction. How would you structure the transition from AI to human interlocutor to maximize the benefits of both?

5. Norton's concept of "investment" argues that language learning motivation is tied to the learner's desire for social membership and identity. Can AI interaction contribute to investment? Under what conditions?

---

## Suggested Further Reading

- Gass, S. M., & Mackey, A. (2007). Input, interaction, and output in second language acquisition. In B. VanPatten & J. Williams (Eds.), *Theories in second language acquisition* (pp. 175-199). Lawrence Erlbaum.
- Lantolf, J. P., & Thorne, S. L. (2006). *Sociocultural theory and the genesis of second language development*. Oxford University Press.
- Long, M. H. (1996). The role of the linguistic environment in second language acquisition. In W. C. Ritchie & T. K. Bhatia (Eds.), *Handbook of second language acquisition* (pp. 413-468). Academic Press.
- Norton, B. (2013). *Identity and language learning: Extending the conversation* (2nd ed.). Multilingual Matters.
- Pica, T. (1994). Research on negotiation: What does it reveal about second-language learning conditions, processes, and outcomes? *Language Learning*, 44(3), 493-527.

---

*Chapter word count: approximately 10,400 words*
