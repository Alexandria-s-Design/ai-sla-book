# Chapter 10: Pronunciation, Phonology, and Speech Technology

## Introduction: The Spoken Dimension of Second Language Acquisition

Of all the competencies that second language learners must develop, pronunciation occupies a uniquely fraught position. It is the most immediately perceptible marker of non-nativeness, the dimension most subject to social judgment, and--paradoxically--the component most frequently neglected in both SLA research and language pedagogy (Derwing & Munro, 2015). For decades, pronunciation instruction suffered from what Levis (2005) described as a theoretical vacuum: teachers either drilled minimal pairs in the audiolingual tradition or avoided pronunciation altogether, having internalized the Krashenian assumption that phonological competence would emerge naturally from sufficient comprehensible input. Neither approach was well supported by evidence, and neither served learners adequately.

Into this vacuum has arrived a suite of artificial intelligence technologies that promise to transform pronunciation instruction. Automatic speech recognition (ASR) systems can now transcribe learner speech in real time, identify segmental and suprasegmental deviations, and provide immediate corrective feedback. Text-to-speech (TTS) engines generate naturalistic spoken input in dozens of languages and varieties. AI-powered pronunciation coaches--ELSA Speak, SpeechAce, Speechling, and features embedded in platforms like Duolingo and Rosetta Stone--claim to offer personalized, infinitely patient pronunciation training that adapts to individual learner profiles. The marketing narratives surrounding these tools are seductive: learn to speak like a native, anywhere, anytime, without the social anxiety of face-to-face interaction.

This chapter subjects those claims to rigorous scrutiny. It begins by reviewing the theoretical foundations of L2 phonological acquisition, establishing what we know about how learners perceive and produce the sounds of a new language. It then examines the technical architecture and capabilities of ASR and TTS systems, assessing what these technologies can and cannot detect, model, and teach. The chapter evaluates the empirical evidence on ASR-based pronunciation training, which is more equivocal than commercial marketing suggests. It then turns to what may be the most consequential issue in AI-mediated pronunciation instruction: the question of whose pronunciation norms these systems encode, and what happens when algorithmic standards of "correctness" collide with the sociolinguistic reality of World Englishes and pluricentric language varieties. Throughout, the chapter maintains the critical-then-affordances orientation established in earlier chapters: we must understand the limitations before we can responsibly leverage the capabilities.

---

## 10.1 Theoretical Foundations: How L2 Phonology Is Acquired

### 10.1.1 The Challenge of L2 Sound Systems

The acquisition of a second language phonological system presents learners with challenges that are qualitatively different from those encountered in morphosyntax or lexis. By the end of the first year of life, infants have already undergone perceptual narrowing--the process by which sensitivity to phonetic contrasts not present in the ambient language declines dramatically (Werker & Tees, 1984; Kuhl et al., 2006). This early perceptual reorganization means that adult L2 learners approach a new sound system with a perceptual apparatus already tuned to their first language. They do not hear the L2 as it is; they hear it through the filter of their L1 phonological categories.

This fundamental insight--that L2 perception is mediated by L1 categories--has generated the field's two most influential theoretical models. Understanding these models is essential before evaluating whether AI systems can intervene effectively in phonological acquisition, because the models specify different mechanisms of difficulty and therefore imply different pedagogical targets.

### 10.1.2 Flege's Speech Learning Model

James Emil Flege's Speech Learning Model (SLM), first articulated in 1995 and substantially revised as the SLM-r (Flege & Bohn, 2021), proposes that the difficulty of acquiring L2 sounds is determined by their perceived relationship to existing L1 categories. The model's central claim is counterintuitive: L2 sounds that are phonetically similar to L1 categories are harder to acquire than sounds that are entirely novel. This is because similar sounds are perceptually assimilated to the nearest L1 category, preventing the learner from establishing a separate phonetic representation. Novel sounds, by contrast, have no L1 attractor and can be more readily perceived as distinct, allowing the formation of new categories.

The SLM-r makes several predictions directly relevant to AI pronunciation systems. First, it predicts that perception precedes production--learners cannot produce contrasts they cannot perceive. This implies that AI pronunciation tools focusing exclusively on production feedback (as most do) may be targeting the wrong end of the process. Second, the model predicts that L1-L2 phonetic similarity determines the trajectory of acquisition, which means that effective AI pronunciation training would need to be sensitive to each learner's specific L1 background. A Japanese learner's difficulty with English /r/-/l/ reflects a fundamentally different perceptual challenge than a Spanish learner's difficulty with English /b/-/v/, and a pronunciation AI that treats both as generic "mispronunciations" misses the theoretical point entirely.

Third, the SLM-r emphasizes that phonetic categories are dynamic and continue to evolve across the lifespan. This is a hopeful prediction for adult learners, contradicting the strong version of the Critical Period Hypothesis. It also implies that sustained exposure and practice--exactly what AI tools can provide--may facilitate ongoing phonetic category formation, provided the input and feedback are appropriately structured.

### 10.1.3 Best's Perceptual Assimilation Model

Catherine Best's Perceptual Assimilation Model (PAM; Best, 1995; Best & Tyler, 2007) complements the SLM by providing a more detailed account of how naive listeners--those with no experience of a given L2--initially perceive non-native contrasts. PAM categorizes L2 sound pairs according to how they map onto L1 articulatory gestures, yielding several assimilation types: Two-Category assimilation (each L2 sound maps to a different L1 category, making discrimination easy), Single-Category assimilation (both L2 sounds map to the same L1 category, making discrimination difficult), and Category-Goodness assimilation (both map to one L1 category but differ in how well they exemplify it, yielding intermediate discrimination).

PAM's predictions have direct implications for AI pronunciation assessment. An ASR system that simply flags a sound as "incorrect" provides no information about the perceptual assimilation pattern that produced the error. A learner who assimilates both English /θ/ and /s/ to a single L1 sibilant category (Single-Category assimilation) needs perceptual training before production practice will be effective. An AI system that provides production feedback without addressing the underlying perceptual confusion is, from a PAM perspective, pedagogically premature.

### 10.1.4 The Intelligibility-Comprehensibility-Accentedness Framework

Perhaps the most consequential theoretical contribution to pronunciation pedagogy in the past three decades has been the empirical distinction among intelligibility, comprehensibility, and accentedness, established through the extensive research program of Tracey Derwing and Murray Munro (Derwing & Munro, 1997, 2009, 2015; Munro & Derwing, 1995). Their work demonstrates that these three constructs, while related, are partially independent: a speaker can be heavily accented yet highly intelligible, and the correlation between accentedness and comprehensibility is weaker than intuition suggests.

This distinction has profound implications for AI pronunciation systems. If the goal of pronunciation instruction is intelligibility and comprehensibility rather than accent elimination--as the professional consensus now holds (Levis, 2005; Derwing & Munro, 2015)--then AI systems should be evaluated on whether they improve functional communication rather than whether they bring learner speech closer to a monolingual native speaker norm. As we shall see, most current ASR-based pronunciation tools do not make this distinction. They evaluate pronunciation against a single target variety (typically General American English or Received Pronunciation) and generate feedback oriented toward accent reduction rather than intelligibility enhancement. This is not merely a technical limitation; it is a theoretical and ideological choice with consequences for learners.

### 10.1.5 Suprasegmental Phonology and the Primacy of Prosody

A growing body of research indicates that suprasegmental features--stress, rhythm, intonation, and connected speech phenomena--contribute more to intelligibility and comprehensibility than individual segmental accuracy (Hahn, 2004; Kang, Rubin, & Pickering, 2010; Derwing, Munro, & Wiebe, 1998). Misplaced lexical stress, inappropriate sentence-level intonation, and failure to reduce unstressed syllables create more communicative disruption than the substitution of one phoneme for another. Derwing et al. (1998) found that learners who received suprasegmental-focused instruction improved more in comprehensibility ratings than those who received segmental instruction alone.

This finding presents a significant challenge for AI pronunciation systems. Historically, ASR technology has been far more capable of evaluating segmental accuracy--whether a given phoneme matches a target--than of analyzing prosodic features such as pitch contour, stress placement, speech rhythm, and intonation patterns. While recent advances in deep learning have improved prosody analysis, the gap between segmental and suprasegmental assessment capabilities remains substantial in commercial pronunciation applications. The pedagogical risk is that AI pronunciation tools may inadvertently reinforce a segmental bias in pronunciation instruction, directing learner attention toward phoneme-level accuracy at the expense of the suprasegmental features that matter more for communication.

---

## 10.2 Automatic Speech Recognition: Architecture, Capabilities, and Limitations

### 10.2.1 How ASR Systems Work

To evaluate AI pronunciation tools critically, language educators and researchers must understand, at a conceptual level, how automatic speech recognition operates. Modern ASR systems have undergone a fundamental architectural shift from the hidden Markov models (HMMs) and Gaussian mixture models (GMMs) that dominated the field through the 2000s to end-to-end deep learning approaches based on recurrent neural networks, transformers, and connectionist temporal classification (Graves, Mohamed, & Hinton, 2013; Gulati et al., 2020).

The most influential recent ASR system, OpenAI's Whisper (Radford et al., 2023), exemplifies the current state of the art. Whisper is a transformer-based encoder-decoder model trained on 680,000 hours of multilingual speech data scraped from the internet. It achieves near-human transcription accuracy on standard benchmarks for high-resource languages and demonstrates robust performance on accented speech, noisy environments, and code-switched utterances. Whisper's architecture processes raw audio spectrograms through a series of transformer encoder layers, producing contextual representations that are then decoded into text tokens.

For pronunciation assessment, however, transcription accuracy is a misleading metric. A transcription-oriented ASR system is optimized to figure out what the speaker *intended* to say, actively compensating for pronunciation variation, accent, and disfluency. A pronunciation assessment system, by contrast, must do the opposite: it must detect and characterize deviations from a target pronunciation norm. These are fundamentally different tasks, and an ASR system that is excellent at the former may be poorly suited to the latter.

### 10.2.2 ASR for Pronunciation Assessment: The Goodness of Pronunciation Framework

The most widely researched approach to ASR-based pronunciation assessment is the Goodness of Pronunciation (GOP) framework, first proposed by Witt and Young (2000). GOP scoring computes the log-posterior probability that a given speech segment corresponds to the expected phoneme in a forced-alignment paradigm. The learner reads a known text, the ASR system aligns the audio to the expected phoneme sequence, and each phoneme receives a score indicating how closely it matches native speaker models. Low GOP scores flag potential pronunciation errors.

The GOP approach has several well-documented limitations. First, it requires read-aloud speech, limiting its applicability to spontaneous conversation. Second, it evaluates pronunciation at the phoneme level, with limited capacity for suprasegmental assessment. Third, and most critically, the "goodness" in GOP is defined relative to a training corpus of native speaker speech, which means that the system's pronunciation norms are entirely determined by whose speech was used in training. If the training data consists primarily of General American English speakers from the Midwest, the system will flag as deviant any pronunciation that differs from that variety--including other native English varieties (Kachru, 1985).

### 10.2.3 The L1 Background Problem

One of the most significant limitations of current ASR-based pronunciation systems is their inconsistent performance across learner L1 backgrounds. Numerous studies have demonstrated that ASR accuracy degrades significantly for non-native speakers, with the degree of degradation varying by L1 (Gretter, Matassoni, Falavigna, & Dalmasso, 2020; Radzikowski, Wang, Yoshie, & Kashino, 2019). This means that the learners who most need pronunciation support--those whose L1 phonological systems are most distant from the target language--receive the least accurate assessment.

The problem is structural. ASR systems learn from their training data, and if that data is dominated by native speakers and speakers from certain L1 backgrounds (typically Mandarin, Spanish, and Arabic, which are well-represented in L2 English corpora), the system will be more adept at recognizing and assessing the speech patterns of those groups. Learners from underrepresented L1 backgrounds--Tagalog, Yoruba, Bengali, Thai--may find that the system cannot accurately transcribe their speech, let alone provide meaningful pronunciation feedback. This is not a bug that will be fixed with more data; it is a reflection of the economic incentive structures that determine which languages and varieties receive investment in speech technology.

### 10.2.4 Beyond Phoneme Detection: Prosody Analysis in ASR

Recent advances have expanded ASR-based assessment beyond segmental phoneme evaluation to include prosodic features. Systems such as SpeechAce and ELSA Speak now claim to evaluate stress placement, intonation contour, speech rate, and rhythm. The technical approaches vary: some use pitch tracking algorithms (via fundamental frequency extraction) combined with duration and intensity measurements; others employ neural network classifiers trained on prosodic features extracted from native speaker corpora.

The accuracy of these prosodic assessments is considerably lower than that of segmental assessments. Intonation evaluation, in particular, remains challenging because intonation is highly context-dependent, speaker-variable, and functionally complex. A rising pitch at the end of an utterance might signal a question, uncertainty, continuation, or a discourse-level function like list intonation--and the "correctness" of the pattern depends on communicative intent, which the ASR system cannot access. Current prosody assessment systems tend to evaluate surface-level acoustic features (pitch range, pitch contour shape, duration ratios) without reference to the communicative function of the prosodic choice, yielding feedback that is, at best, incomplete and, at worst, misleading.

---

## 10.3 Text-to-Speech: AI-Generated Input for Pronunciation Learning

### 10.3.1 The Evolution of TTS Technology

Text-to-speech technology has undergone a revolution comparable to that in ASR. Early TTS systems (DECtalk, Festival) produced robotic, immediately identifiable synthetic speech that bore little resemblance to human vocal production. The current generation of neural TTS systems--including Google's WaveNet (van den Oord et al., 2016), Microsoft's VALL-E (Wang et al., 2023), OpenAI's TTS models, and ElevenLabs' voice synthesis platform--generates speech that is, in many contexts, perceptually indistinguishable from human speech. These systems model not only segmental accuracy but prosodic variation, speaker-specific vocal quality, emotional affect, and naturalistic disfluency patterns.

For language learning, high-quality TTS serves a fundamentally different function than ASR. While ASR evaluates learner production, TTS provides input--the spoken models against which learners calibrate their perception and production. From an SLA theoretical perspective, TTS is an input technology, and its value should be assessed against the criteria established in Chapter 4: Does it provide comprehensible input at an appropriate level? Does it expose learners to the phonological features they need to acquire? Does it support the kind of attentional engagement that Schmidt's (1990) Noticing Hypothesis identifies as necessary for acquisition?

### 10.3.2 TTS as a Model for Pronunciation

The use of TTS as a pronunciation model raises several theoretical and practical questions. First, there is the question of input quality. If TTS-generated speech is perceptually indistinguishable from human speech, does it function equivalently as input for phonological acquisition? The limited research available suggests that learners can improve perception of specific phonological contrasts through exposure to high-quality synthetic speech (Bione & Cardoso, 2020), though the evidence base is thin and the generalizability to diverse L1-L2 pairings remains uncertain.

Second, there is the question of variability. Natural speech input exhibits substantial within-speaker and between-speaker variability in phonetic realization--a feature that phonological learning theory suggests is actually beneficial. High-variability phonetic training (HVPT), in which learners are exposed to the same phonological contrast produced by multiple speakers in varied phonetic contexts, has been shown to promote more robust perceptual category formation than training with a single speaker (Logan, Lively, & Pisoni, 1991; Thomson, 2011). TTS systems can generate speech in multiple synthetic voices, potentially replicating the variability of HVPT paradigms. However, the distribution of phonetic variation in TTS-generated speech may differ systematically from that of natural human speech, and whether this difference matters for perceptual learning is an open empirical question.

### 10.3.3 TTS for Listening Discrimination and Perceptual Training

One of the most promising applications of TTS in pronunciation instruction is the generation of perceptual training stimuli. If, as the SLM and PAM predict, perception is the gateway to production, then systematic perceptual training should precede production practice. TTS enables the creation of large stimulus sets for minimal pair discrimination, vowel space exploration, and prosodic contour identification, customized to target the specific contrasts predicted to be difficult for learners of a given L1 background.

Thomson (2011, 2012) developed the English Accent Coach, which uses natural speech stimuli for HVPT-based vowel perception training and has demonstrated significant perceptual and productive improvements for L2 English learners. The principles underlying this approach--high variability, multiple speakers, immediate feedback, spaced repetition--could be implemented at scale using TTS-generated stimuli, potentially making HVPT available for a far wider range of L1-L2 pairings than the labor-intensive collection of natural speech recordings would allow. This is an area where AI technology offers a genuine affordance that is well-aligned with theoretical predictions, though empirical validation with TTS-generated stimuli specifically remains necessary.

### 10.3.4 Voice Cloning and Personalized Pronunciation Models

An emerging TTS capability with intriguing pedagogical potential is voice cloning--the ability to generate speech in a specific individual's voice from a small sample of their natural speech. Systems such as ElevenLabs and Microsoft's VALL-E can produce high-fidelity voice clones from as little as three seconds of reference audio. For pronunciation instruction, this raises the possibility of generating target-language speech in the learner's own voice, allowing them to hear "themselves" speaking the L2 with target-like pronunciation.

The theoretical rationale for this approach draws on research suggesting that self-related processing enhances attention and memory (Symons & Johnson, 1997) and that perceptual-motor links between hearing one's own voice and articulating speech may facilitate the perception-production bridge that SLM identifies as critical. However, this application also raises significant ethical concerns regarding voice consent, deepfake potential, and the psychological impact of hearing one's own voice producing speech patterns that may be unattainable. These are not hypothetical concerns; they are active considerations as voice cloning technology becomes more accessible and pronunciation app developers explore its integration.

---

## 10.4 AI Pronunciation Coaching: Current Systems and Their Pedagogical Architecture

### 10.4.1 The Landscape of AI Pronunciation Tools

The commercial landscape of AI pronunciation tools has expanded rapidly since 2020. A critical evaluation requires distinguishing among several categories of systems, each with different technical architectures and pedagogical approaches.

**Dedicated pronunciation apps** such as ELSA Speak, SpeechAce, and Speechling focus exclusively on pronunciation improvement. ELSA Speak (English Language Speech Assistant) uses a proprietary deep learning ASR engine trained specifically on non-native English speech from speakers of 100+ L1 backgrounds. It provides phoneme-level scoring, visual feedback (spectrograms, waveform comparisons), and adaptive lesson sequencing. SpeechAce offers pronunciation scoring via an API used by other educational platforms, providing GOP-style phoneme scores and prosodic ratings. Speechling combines ASR-based automated feedback with delayed human coach feedback, representing a hybrid model.

**General language learning platforms** including Duolingo, Rosetta Stone, Babbel, and Busuu incorporate pronunciation assessment as one feature among many. These platforms typically use third-party ASR engines (often Google's Speech-to-Text API) with proprietary scoring layers on top. The pronunciation feedback is generally less granular than that of dedicated tools, often providing only a binary correct/incorrect judgment or a holistic score rather than phoneme-level analysis.

**LLM-based conversational practice tools** such as Speak (formerly SpeakEasy), ChatGPT Advanced Voice Mode, and various LLM-powered tutoring platforms now offer spoken interaction with real-time pronunciation feedback. These represent the most recent evolution, combining ASR for speech input, LLM for conversational management and feedback generation, and TTS for spoken output. The pronunciation feedback in these systems tends to be contextual and communicatively oriented rather than drill-based, which aligns better with current pronunciation pedagogy but may lack the systematic targeting of specific phonological features that dedicated tools provide.

### 10.4.2 Feedback Modalities in AI Pronunciation Systems

AI pronunciation tools employ various feedback modalities, and the pedagogical effectiveness of each is an empirical question that intersects with broader SLA research on corrective feedback (see Chapter 7). Common modalities include:

**Visual feedback** encompasses spectrogram displays, pitch contour visualizations, waveform comparisons between learner and model utterances, and animated articulatory diagrams (sagittal section views showing tongue and lip positions). The theoretical rationale draws on research suggesting that visual feedback provides an additional representational channel that can support phonological learning (Olson, 2014), though the evidence is mixed regarding whether learners can effectively interpret spectrographic information without substantial training (Kartushina, Hervais-Adelman, Frauenfelder, & Golestani, 2015).

**Scoring and rating feedback** provides numerical or categorical assessments of pronunciation quality at the phoneme, word, or utterance level. This feedback type aligns with the discrete-point assessment tradition and may promote noticing of specific features (Schmidt, 1990) but risks fragmenting the speech signal in ways that do not reflect natural communication.

**Metalinguistic feedback** provides explicit explanations of pronunciation errors and articulatory instructions (e.g., "Place your tongue between your teeth for the /θ/ sound"). LLM-powered systems can generate contextually rich metalinguistic feedback that goes beyond pre-programmed tips, potentially adapting explanations to the learner's L1 and proficiency level.

**Model comparison feedback** allows learners to hear their own production alongside a model production and visually or auditorily compare the two. This approach leverages the perceptual-motor links central to speech learning but may inadvertently reinforce the native speaker model as the sole target.

### 10.4.3 Adaptive Pronunciation Curricula

The most sophisticated AI pronunciation tools claim to provide adaptive curricula that sequence pronunciation targets based on learner performance data. ELSA Speak, for example, uses a machine learning algorithm to identify each learner's most problematic phonemes and prioritize those in subsequent practice sessions. The adaptive logic draws, implicitly, on Pienemann's (1998) Processability Theory and the notion that instruction should target features at the learner's developmental frontier rather than features that are either already acquired or developmentally premature.

However, the mapping from Processability Theory to pronunciation acquisition is imperfect. While Pienemann's framework provides clear developmental sequences for morphosyntactic features, L2 phonological development does not follow a single universal sequence. The order of difficulty is heavily L1-dependent (as the SLM and PAM predict), and within a given L1-L2 pairing, individual variation in phonological acquisition trajectories is substantial. This means that an adaptive pronunciation system must model not only general L1-based difficulty predictions but also individual learner trajectories, a far more demanding computational task than adapting grammar exercises based on error patterns.

---

## 10.5 Research Evidence on ASR-Based Pronunciation Training

### 10.5.1 Meta-Analyses and Systematic Reviews

The empirical evidence on ASR-based pronunciation training has been synthesized in several systematic reviews and meta-analyses. Lee, Jang, and Plonsky (2015) conducted a meta-analysis of technology-mediated pronunciation instruction and found a small-to-medium overall effect (d = 0.44) for ASR-based tools on pronunciation improvement. Critically, the effects were larger for controlled (read-aloud) speech than for spontaneous speech, larger for segmental features than for suprasegmentals, and larger for perception than for production.

Fouz-Gonzalez (2020) reviewed studies on ASR-based pronunciation training and identified several methodological concerns that temper the positive findings: small sample sizes, lack of delayed posttests, inconsistent operationalization of pronunciation improvement, and reliance on the ASR system's own scoring as the outcome measure (a circularity problem). When human raters rather than ASR scores served as the criterion measure, the effects were notably smaller.

More recently, Luo (2024) conducted a meta-analysis specifically examining AI-powered pronunciation tools published between 2018 and 2023, finding a moderate positive effect (g = 0.56) on pronunciation accuracy as measured by human raters, but with substantial heterogeneity across studies. Treatment duration, L1 background, and the specific AI tool used moderated effects significantly. Notably, studies with active control groups (receiving non-AI pronunciation instruction) showed smaller effects than those comparing AI treatment to no pronunciation instruction at all--a finding that suggests AI tools may not be superior to human pronunciation instruction but may be effective when such instruction is unavailable.

### 10.5.2 Perception Versus Production Effects

A consistent finding across studies is that ASR-based pronunciation tools produce stronger effects on perception than on production (Lee et al., 2015; Thomson & Derwing, 2015). This aligns with the SLM's prediction that perceptual category formation precedes productive mastery but complicates the value proposition of tools that primarily provide production feedback. If the perception-production link is the critical pathway, then AI tools that focus on perceptual training (discrimination tasks, identification tasks, HVPT) may be more effective than those that focus on production practice with ASR feedback, though such tools are rarer in the commercial market because production practice is more engaging and marketable.

### 10.5.3 Learner Variables and Differential Effectiveness

Research increasingly suggests that ASR-based pronunciation training is not equally effective for all learners. Proficiency level appears to moderate effects: intermediate learners tend to benefit more than beginners (who lack the metalinguistic awareness to interpret pronunciation feedback) or advanced learners (whose pronunciation patterns may be more resistant to change). L1 background interacts with tool effectiveness in predictable ways: learners whose L1 phonological systems share more features with the target language show greater improvement, likely because the ASR system is more accurate for their speech and the phonological distance to be traversed is smaller.

Motivational and affective variables also play a role. Learners who report high pronunciation anxiety may benefit particularly from AI pronunciation practice because it removes the social evaluation component of face-to-face interaction (Mroz, 2020). The affective filter construct, though theoretically contested (see Chapter 2), may have particular relevance in the pronunciation domain, where the embodied, identity-laden nature of speech makes social anxiety a more powerful inhibitor than in written language production. AI pronunciation tools may lower affective barriers not because they are better teachers than humans, but because they are less socially threatening interlocutors.

### 10.5.4 The Transfer Problem

Perhaps the most significant empirical question about ASR-based pronunciation training is whether improvements transfer to spontaneous speech. Most pronunciation apps assess and train pronunciation through controlled tasks: read-aloud sentences, word lists, minimal pair drills, and scripted dialogues. The evidence for transfer from controlled practice to spontaneous speech is limited and sobering. Derwing and Munro (2015) have long argued that pronunciation gains in controlled speech do not automatically transfer to communicative interaction, and this concern is amplified in the AI context where the entire practice environment is controlled.

Several studies have investigated transfer effects directly. Liakin, Cardoso, and Liakina (2015) found that mobile ASR-based pronunciation practice improved production of target French vowels in read-aloud tasks but showed limited transfer to picture-description tasks requiring spontaneous speech. Elimat and AbuSeileek (2014) reported similar patterns for English pronunciation among Arabic L1 learners. The transfer problem is not unique to AI pronunciation tools--it is a perennial challenge in pronunciation pedagogy--but the highly structured, controlled-practice orientation of most AI tools may exacerbate it.

---

## 10.6 The Native Speaker Fallacy in AI Pronunciation Systems

### 10.6.1 Whose Standard?

The most fundamental critique of AI pronunciation systems concerns the pronunciation norms they encode. Every ASR-based pronunciation assessment system must have a target--a model of "correct" pronunciation against which learner speech is evaluated. In virtually all commercial pronunciation tools for English, this target is an idealized monolingual native speaker variety, typically General American English or, less commonly, Received Pronunciation. The choice is rarely made explicit to users, and the systems present their feedback as objective measures of pronunciation "accuracy" or "quality" rather than as comparisons to one particular sociolinguistic variety among many.

This encoding of a single native speaker standard as the benchmark of correctness reflects what Phillipson (1992) termed the "native speaker fallacy"--the assumption that the native speaker represents the ultimate model and measure of language proficiency. Decades of sociolinguistic and applied linguistic scholarship have challenged this assumption (Canagarajah, 1999; Cook, 1999; Holliday, 2006; Kumaravadivelu, 2016), yet it persists in AI pronunciation systems, embedded in training data, scoring algorithms, and feedback design.

The consequences are not trivial. A learner of English whose speech is intelligible and comprehensible to a wide range of interlocutors but whose pronunciation retains features of their L1 variety may receive consistently negative feedback from an AI system calibrated to General American norms. This feedback tells the learner, implicitly but powerfully, that their way of speaking English is deficient--a message with significant implications for linguistic identity, investment in learning, and attitudes toward one's own L1 (Norton, 2013; see Chapter 12). The AI system, by virtue of its apparently objective, algorithmic authority, may carry more weight than a human teacher who could contextualize pronunciation feedback within a broader understanding of communicative competence.

### 10.6.2 The Training Data Problem

The native speaker bias in AI pronunciation systems is, in the first instance, a training data problem. ASR systems learn to recognize and evaluate speech from the speech data they are trained on. If the training data consists primarily of native speakers of a prestige variety, the system will develop acoustic models that treat that variety as canonical and evaluate all other speech against it. Non-native speech that diverges from these models will receive lower scores, regardless of its communicative effectiveness.

This is not an inevitable consequence of the technology. It is a design choice, driven by the availability of large, well-annotated speech corpora (which are disproportionately available for prestige varieties of major world languages) and by market assumptions about what language learners want (which are shaped by, and in turn reinforce, native-speakerist ideology). It is technically possible to train ASR systems on diverse varieties--including L2 varieties--and to calibrate pronunciation assessment against intelligibility rather than native-likeness. Some research prototypes have demonstrated this approach (Derwing, Munro, & Thomson, 2007; Isaacs & Thomson, 2014), but commercial products have been slow to adopt it, in part because "speak like a native" sells better than "be understood by diverse interlocutors."

### 10.6.3 Ideological Reproduction Through Technology

The embedding of native speaker norms in AI pronunciation systems exemplifies a broader pattern identified by critical technology scholars: technology does not merely reflect social values; it reproduces and reinforces them (Winner, 1980; Noble, 2018). When an AI pronunciation system flags a learner's Indian English rhotic patterns or Nigerian English vowel qualities as "errors," it is performing an ideological act--classifying certain varieties as standard and others as deviant--under the guise of neutral technological assessment. The algorithmic medium obscures the social judgments embedded in the system, making them appear as objective facts about language rather than contingent choices about which varieties to privilege.

Ruecker and Ives (2015) have documented how the authority of technology can amplify native-speakerist ideologies in language education, and AI pronunciation systems represent a particularly potent vector for this amplification. Unlike a human teacher, who might be challenged, questioned, or persuaded to adopt a more pluralistic stance, an AI system's pronunciation judgments are experienced as computational facts. The learner cannot negotiate with the algorithm or ask it to recognize their variety as legitimate. The feedback is, in Foucault's (1977) terms, a form of disciplinary power: it normalizes a particular linguistic standard through continuous, individualized assessment that the learner experiences as objective self-improvement.

---

## 10.7 World Englishes and Pluricentric Perspectives on Pronunciation AI

### 10.7.1 The Kachruvian Framework and AI

Braj Kachru's (1985) Three Circles model--distinguishing Inner Circle (English as a native language), Outer Circle (English as a second language with institutional functions), and Expanding Circle (English as a foreign language) countries--provides a useful framework for examining the implications of AI pronunciation systems. The model highlights that the majority of English speakers worldwide are not Inner Circle speakers, and that Outer Circle varieties (Indian English, Nigerian English, Singaporean English, Philippine English) are established, systematic varieties with their own phonological norms, not "deficient" versions of Inner Circle standards.

AI pronunciation systems that evaluate all English speech against Inner Circle norms effectively delegitimize Outer Circle varieties. A speaker of Indian English who uses retroflex consonants, follows Indian English stress patterns, and employs Indian English intonation contours is speaking a recognized variety of English with its own internal consistency. An AI system that marks these features as errors is not identifying pronunciation problems; it is imposing one variety's norms on speakers of another variety. The pedagogical and ideological implications differ dramatically depending on the learner's context: an Expanding Circle learner seeking to communicate primarily with Inner Circle speakers may benefit from feedback oriented toward those norms, while an Outer Circle speaker or a learner in a lingua franca context may be poorly served or actively harmed.

### 10.7.2 Jenkins' Lingua Franca Core

Jennifer Jenkins' (2000) Lingua Franca Core (LFC) represents the most developed attempt to identify the phonological features that are essential for mutual intelligibility in English as a Lingua Franca (ELF) contexts--contexts in which most English communication now occurs. The LFC specifies a subset of phonological features (including most consonants, consonant clusters, vowel length distinctions, and nuclear stress placement) while identifying other features (such as dental fricatives, vowel quality differences in certain positions, and weak forms) as non-core--not essential for intelligibility and therefore not appropriate targets for instruction in ELF contexts.

The LFC provides a principled basis for configuring AI pronunciation systems. Rather than evaluating all phonological features against a native speaker standard, a pronunciation AI calibrated to the LFC would focus feedback on the features most critical for intelligibility while accepting variation in non-core features. This approach would reduce unnecessary and potentially harmful feedback, honor the legitimacy of diverse English varieties, and orient pronunciation instruction toward communicative effectiveness rather than native-like conformity.

To date, no major commercial pronunciation AI system has implemented a Lingua Franca Core approach. The technological barriers are minimal--the distinction between core and non-core features could be implemented as a scoring filter on existing ASR output. The barriers are ideological and commercial: the native speaker standard sells, and the concept of "good enough" pronunciation is harder to market than the promise of "perfect" pronunciation. This represents a clear case where the technology is capable of supporting a more equitable pedagogical approach but market forces and native-speakerist ideology prevent its adoption.

### 10.7.3 Beyond English: Pluricentric Languages and AI

The issues raised by World Englishes perspectives apply with equal or greater force to other pluricentric languages--languages with multiple recognized standard varieties. Spanish, French, Portuguese, Arabic, and Chinese all exhibit significant phonological variation across national and regional varieties. A Spanish pronunciation AI trained on Castilian Spanish will evaluate Latin American Spanish features as errors; a French pronunciation tool calibrated to Metropolitan French will flag Quebec French or West African French pronunciations as deviant; a Chinese pronunciation system trained on Standard Mandarin will penalize speakers of Southern Mandarin varieties for features such as the merger of /n/ and /l/ or the absence of retroflex initials.

For less commonly taught languages (LCTLs), the problem is compounded by data scarcity. Pronunciation AI systems require large speech corpora for training, and for languages with fewer digital resources, the available corpora may represent only one variety--typically the prestige variety of the most economically powerful nation where the language is spoken. This means that AI pronunciation tools for LCTLs may not only impose a single standard but impose it without the possibility of alternative models, because the speech data for other varieties simply does not exist in sufficient quantity.

---

## 10.8 Pedagogical Implications: Integrating AI Speech Technology Responsibly

### 10.8.1 A Framework for AI Pronunciation Integration

Drawing on the theoretical analysis and empirical evidence reviewed in this chapter, we can articulate a set of principles for integrating AI speech technology into pronunciation instruction responsibly and effectively.

**Principle 1: Perception before production.** Consistent with the SLM and PAM, AI pronunciation instruction should begin with perceptual training (using TTS-generated stimuli and discrimination tasks) before moving to production practice with ASR feedback. This sequence aligns with the theoretical prediction that perceptual category formation is a precondition for productive improvement and addresses the finding that ASR feedback on production may be premature for learners who have not yet developed the perceptual categories needed to interpret that feedback.

**Principle 2: L1-specific targeting.** AI pronunciation systems should leverage learner L1 information to predict which phonological contrasts will be most challenging and to sequence instruction accordingly. The SLM's predictions about which L2 sounds will be difficult for speakers of specific L1s are well-established and could be operationalized in adaptive pronunciation curricula. A generic one-size-fits-all pronunciation curriculum wastes learner time on features that are not problematic for their L1 background and may miss features that are.

**Principle 3: Suprasegmental priority.** Given the research evidence that suprasegmental features contribute more to intelligibility than segmental accuracy, AI pronunciation instruction should prioritize stress, rhythm, and intonation alongside--or even before--individual sound production. While AI systems' suprasegmental assessment capabilities are less mature than their segmental capabilities, the pedagogical priority should drive technological development rather than the reverse.

**Principle 4: Intelligibility orientation.** AI pronunciation feedback should be calibrated to intelligibility and comprehensibility rather than native-likeness. This requires moving beyond binary correct/incorrect scoring to graduated assessments that distinguish between features that impair intelligibility and features that contribute to accent without affecting communication. Levis's (2005) nativeness versus intelligibility principles provide the theoretical grounding.

**Principle 5: Variety awareness.** AI pronunciation tools should make their target variety explicit, offer multiple target varieties where possible, and allow learners and teachers to configure the system according to their communicative context. A learner preparing for academic study in the United Kingdom has different pronunciation targets than one preparing for business communication in Southeast Asia, and the same AI system should be able to accommodate both contexts.

**Principle 6: Transfer-oriented practice.** To address the transfer problem, AI pronunciation practice should be embedded in communicative tasks that require spontaneous speech, not limited to read-aloud drills. LLM-powered conversational practice tools have the potential to provide this communicative context, assessing pronunciation within the flow of meaningful interaction rather than in isolated drill exercises.

### 10.8.2 Hybrid Models: AI and Human Teachers

The most effective approach to pronunciation instruction is likely a hybrid one that leverages the strengths of both AI systems and human teachers while compensating for each other's limitations. AI pronunciation tools excel at providing unlimited patient practice, immediate feedback on segmental features, systematic coverage of phoneme inventories, and anxiety-reduced practice environments. Human teachers excel at contextualizing pronunciation within communicative goals, adapting instruction to individual learner needs in real time, addressing the social and identity dimensions of pronunciation, and making pedagogical judgments about when native-like pronunciation is a reasonable goal and when intelligibility is sufficient.

A practical hybrid model might proceed as follows: the AI system conducts an initial diagnostic assessment to identify the learner's most problematic features (weighted by their impact on intelligibility); the human teacher reviews the diagnostic, selects priority targets, and discusses pronunciation goals with the learner; the learner practices targeted features with the AI system between class sessions; the human teacher monitors AI-generated performance data, provides communicative practice contexts in class, and addresses prosodic and discourse-level pronunciation issues that the AI cannot adequately assess. This model preserves the human teacher's role as pedagogical decision-maker while leveraging the AI system's capacity for sustained, individualized practice.

### 10.8.3 Critical Literacy in AI Pronunciation

A final pedagogical imperative is the development of critical digital literacy around AI pronunciation tools. Learners should understand that pronunciation AI embodies specific linguistic norms, that these norms are not neutral or universal, and that a low score from a pronunciation AI does not necessarily indicate a communication problem. This kind of critical awareness is particularly important for learners from Outer Circle contexts or learners of pluricentric languages who may encounter AI feedback that pathologizes their native or near-native variety.

Teachers play an essential role in fostering this critical literacy. They can facilitate discussions about language variation and standard language ideology, help learners interpret AI pronunciation feedback in light of their communicative goals, and explicitly address the question of whose English (or Spanish, or French, or Arabic) the AI system is evaluating against. Without this critical framing, AI pronunciation tools risk reinforcing exactly the kind of native-speakerist ideology that applied linguistics has spent decades dismantling.

---

## 10.9 Future Directions: Toward Equitable, Theory-Informed Speech Technology

### 10.9.1 Intelligibility-Based ASR Assessment

The most important technical development needed in AI pronunciation systems is the shift from native-likeness to intelligibility as the assessment criterion. This requires not merely recalibrating existing systems but fundamentally rethinking the assessment construct. An intelligibility-based ASR system would need to model not a single speaker norm but a range of listener perceptions, evaluating whether a given pronunciation is likely to be understood by diverse interlocutors rather than whether it matches a native speaker template.

Research prototypes for this approach exist. Isaacs and Thomson (2014) have developed scales for human rater assessment of comprehensibility and accentedness that could inform the design of automated systems. Recent work on listener-oriented ASR evaluation (Zechner et al., 2019) represents steps toward automated intelligibility assessment. However, the computational challenge is substantial: intelligibility is not a property of the speech signal alone but of the interaction between signal, context, and listener, making it inherently more difficult to model than proximity to a single standard.

### 10.9.2 Multimodal Pronunciation Feedback

Future AI pronunciation systems are likely to integrate multiple modalities--audio, visual, and haptic--to provide richer feedback. Ultrasound imaging of tongue movement, electromagnetic articulography, and real-time MRI have been used in research contexts to provide visual feedback on articulatory gestures (Gick, Bernhardt, Bacsfalvi, & Wilson, 2008), and miniaturized, affordable versions of these technologies may become available for consumer pronunciation tools. Haptic feedback (vibrotactile devices that provide tactile information about laryngeal vibration, nasal airflow, or articulatory placement) represents another emerging modality.

The theoretical rationale for multimodal pronunciation feedback is strong. Speech production is an embodied, sensorimotor process, and feedback that engages multiple sensory channels may facilitate the perceptual-motor mapping that underlies phonological acquisition. However, the evidence base for multimodal pronunciation feedback is still nascent, and the risk of cognitive overload from simultaneous visual, auditory, and haptic feedback is real. The optimal combination and sequencing of feedback modalities is an empirical question that deserves sustained research attention.

### 10.9.3 Individualized Pronunciation Goals

Perhaps the most transformative potential of AI in pronunciation instruction lies not in more accurate assessment of a single standard but in the ability to support individualized pronunciation goals. Different learners have different communicative needs, different identity investments in their pronunciation, and different thresholds for how much accent modification they desire. A highly flexible AI pronunciation system could allow learners to set their own goals--ranging from "maximize intelligibility" to "approximate a specific variety" to "maintain my accent while improving specific features that cause misunderstanding"--and calibrate feedback accordingly.

This vision of individualized pronunciation goals aligns with Derwing and Munro's (2015) call for learner-centered pronunciation instruction and with Norton's (2013) emphasis on learner investment and identity (see Chapter 12). It also represents a departure from the current paradigm, in which AI pronunciation tools assume a single goal (native-likeness) and measure all learners against it. The technical infrastructure for this kind of personalization exists; what is needed is a conceptual shift in how pronunciation AI developers think about the purpose of their tools.

---

## 10.10 Conclusion

AI speech technologies--ASR, TTS, and the pronunciation coaching systems built on them--offer genuine affordances for pronunciation instruction. They provide patient, always-available practice partners; they can deliver immediate, individualized feedback on segmental accuracy; they can generate high-quality spoken input for perceptual training; and they can lower the affective barriers that prevent many learners from practicing pronunciation. The empirical evidence, while not as strong as marketing claims suggest, indicates moderate positive effects on pronunciation improvement, particularly for segmental features in controlled speech contexts.

However, these affordances come with significant caveats. Current AI pronunciation systems are better at assessing segments than suprasegmentals, better at evaluating controlled speech than spontaneous production, and better at identifying deviations from a native speaker norm than at assessing communicative intelligibility. Most critically, they embed native speaker norms as the unexamined standard of correctness, reproducing linguistic hierarchies under the guise of objective technological assessment. For learners of World Englishes and pluricentric languages, this ideological encoding can be not merely unhelpful but actively harmful, undermining legitimate varieties and reinforcing discredited native-speakerist assumptions.

The path forward requires not the abandonment of AI speech technology but its realignment with the best available evidence from L2 phonology research and the principled positions of applied linguistics regarding language variation and intelligibility. Perception should precede production. Suprasegmentals should receive at least equal attention as segmentals. Assessment should target intelligibility rather than native-likeness. Multiple target varieties should be available. Learner L1 backgrounds should inform instructional sequencing. And learners should develop critical literacy about the pronunciation norms embedded in the AI tools they use.

The technology is capable of supporting all of these principles. The question is whether market forces, linguistic ideologies, and design inertia will allow that capability to be realized. For language educators, the imperative is clear: use AI pronunciation tools as one resource among many, embed them within a theoretically informed and critically aware pedagogical framework, and never cede to an algorithm the professional judgment about what counts as acceptable, effective, and equitable pronunciation in a given communicative context.

---

## References

Best, C. T. (1995). A direct realist view of cross-language speech perception. In W. Strange (Ed.), *Speech perception and linguistic experience: Issues in cross-language research* (pp. 171-204). York Press.

Best, C. T., & Tyler, M. D. (2007). Nonnative and second-language speech perception: Commonalities and complementarities. In O.-S. Bohn & M. J. Munro (Eds.), *Language experience in second language speech learning* (pp. 13-34). John Benjamins.

Bione, T., & Cardoso, W. (2020). Synthetic speech and L2 pronunciation development. *CALICO Journal*, *37*(3), 281-304.

Canagarajah, A. S. (1999). *Resisting linguistic imperialism in English teaching*. Oxford University Press.

Cook, V. (1999). Going beyond the native speaker in language teaching. *TESOL Quarterly*, *33*(2), 185-209.

Derwing, T. M., & Munro, M. J. (1997). Accent, intelligibility, and comprehensibility: Evidence from four L1s. *Studies in Second Language Acquisition*, *19*(1), 1-16.

Derwing, T. M., & Munro, M. J. (2009). Putting accent in its place: Rethinking obstacles to communication. *Language Teaching*, *42*(4), 476-490.

Derwing, T. M., & Munro, M. J. (2015). *Pronunciation fundamentals: Evidence-based perspectives for L2 teaching and research*. John Benjamins.

Derwing, T. M., Munro, M. J., & Thomson, R. I. (2007). A longitudinal study of ESL learners' fluency and comprehensibility development. *Applied Linguistics*, *29*(3), 359-380.

Derwing, T. M., Munro, M. J., & Wiebe, G. (1998). Evidence in favor of a broad framework for pronunciation instruction. *Language Learning*, *48*(3), 393-410.

Elimat, A. K., & AbuSeileek, A. F. (2014). Automatic speech recognition technology as an effective means for teaching pronunciation. *JALT CALL Journal*, *10*(1), 21-47.

Flege, J. E. (1995). Second language speech learning: Theory, findings, and problems. In W. Strange (Ed.), *Speech perception and linguistic experience* (pp. 233-277). York Press.

Flege, J. E., & Bohn, O.-S. (2021). The revised Speech Learning Model (SLM-r). In R. Wayland (Ed.), *Second language speech learning: Theoretical and empirical progress* (pp. 3-83). Cambridge University Press.

Foucault, M. (1977). *Discipline and punish: The birth of the prison* (A. Sheridan, Trans.). Vintage.

Fouz-Gonzalez, J. (2020). Using technologies for pronunciation instruction: A state-of-the-art review. *CALICO Journal*, *37*(3), 267-280.

Gick, B., Bernhardt, B. M., Bacsfalvi, P., & Wilson, I. (2008). Ultrasound imaging applications in second language acquisition. In J. G. Hansen Edwards & M. L. Zampini (Eds.), *Phonology and second language acquisition* (pp. 309-322). John Benjamins.

Graves, A., Mohamed, A., & Hinton, G. (2013). Speech recognition with deep recurrent neural networks. In *Proceedings of the IEEE International Conference on Acoustics, Speech and Signal Processing* (pp. 6645-6649).

Gretter, R., Matassoni, M., Falavigna, D., & Dalmasso, E. (2020). ASR accuracy for non-native English speakers: A survey. In *Proceedings of the 7th Workshop on NLP for Computer Assisted Language Learning* (pp. 25-33).

Gulati, A., Qin, J., Chiu, C. C., Parmar, N., Zhang, Y., Yu, J., Han, W., Wang, S., Zhang, Z., Wu, Y., & Pang, R. (2020). Conformer: Convolution-augmented transformer for speech recognition. *Interspeech 2020* (pp. 5036-5040).

Hahn, L. D. (2004). Primary stress and intelligibility: Research to motivate the teaching of suprasegmentals. *TESOL Quarterly*, *38*(2), 201-223.

Holliday, A. (2006). Native-speakerism. *ELT Journal*, *60*(4), 385-387.

Isaacs, T., & Thomson, R. I. (2014). Rater experience, rating scale length, and judgments of L2 pronunciation: Revisiting research conventions. *Language Assessment Quarterly*, *10*(2), 135-159.

Jenkins, J. (2000). *The phonology of English as an international language*. Oxford University Press.

Kachru, B. B. (1985). Standards, codification and sociolinguistic realism: The English language in the outer circle. In R. Quirk & H. G. Widdowson (Eds.), *English in the world* (pp. 11-30). Cambridge University Press.

Kang, O., Rubin, D., & Pickering, L. (2010). Suprasegmental measures of accentedness and judgments of language learner proficiency in oral English. *Modern Language Journal*, *94*(4), 554-566.

Kartushina, N., Hervais-Adelman, A., Frauenfelder, U. H., & Golestani, N. (2015). The effect of phonetic production training with visual feedback on the perception and production of foreign speech sounds. *Journal of the Acoustical Society of America*, *138*(2), 817-832.

Kuhl, P. K., Stevens, E., Hayashi, A., Deguchi, T., Kiritani, S., & Iverson, P. (2006). Infants show a facilitation effect for native language phonetic perception between 6 and 12 months. *Developmental Science*, *9*(2), F13-F21.

Kumaravadivelu, B. (2016). The decolonial option in English teaching: Can the subaltern act? *TESOL Quarterly*, *50*(1), 66-85.

Lee, J., Jang, J., & Plonsky, L. (2015). The effectiveness of second language pronunciation instruction: A meta-analysis. *Applied Linguistics*, *36*(3), 345-366.

Levis, J. M. (2005). Changing contexts and shifting paradigms in pronunciation teaching. *TESOL Quarterly*, *39*(3), 369-377.

Liakin, D., Cardoso, W., & Liakina, N. (2015). Learning L2 pronunciation with a mobile speech recognizer: French /y/. *CALICO Journal*, *32*(1), 1-25.

Logan, J. S., Lively, S. E., & Pisoni, D. B. (1991). Training Japanese listeners to identify English /r/ and /l/: A first report. *Journal of the Acoustical Society of America*, *89*(2), 874-886.

Luo, B. (2024). The effectiveness of AI-powered pronunciation training tools: A meta-analysis. *Computer Assisted Language Learning*, *37*(4), 412-438.

Mroz, A. (2020). Seeing voices: Acoustic analyses as evidence for phonological development in L2 interaction. *Studies in Second Language Acquisition*, *42*(5), 951-982.

Munro, M. J., & Derwing, T. M. (1995). Foreign accent, comprehensibility, and intelligibility in the speech of second language learners. *Language Learning*, *45*(1), 73-97.

Noble, S. U. (2018). *Algorithms of oppression: How search engines reinforce racism*. NYU Press.

Norton, B. (2013). *Identity and language learning: Extending the conversation* (2nd ed.). Multilingual Matters.

Olson, D. J. (2014). Benefits of visual feedback on segmental production in the L2 classroom. *Language Learning & Technology*, *18*(3), 173-192.

Phillipson, R. (1992). *Linguistic imperialism*. Oxford University Press.

Pienemann, M. (1998). *Language processing and second language development: Processability Theory*. John Benjamins.

Radford, A., Kim, J. W., Xu, T., Brockman, G., McLeavey, C., & Sutskever, I. (2023). Robust speech recognition via large-scale weak supervision. In *Proceedings of the 40th International Conference on Machine Learning* (pp. 28492-28518).

Radzikowski, K., Wang, L., Yoshie, O., & Kashino, K. (2019). Dual supervised learning framework for non-native speech recognition. *IEEE Access*, *7*, 163567-163576.

Ruecker, T., & Ives, L. (2015). White native English speakers needed: The rhetorical construction of privilege in online teacher recruitment. *TESOL Quarterly*, *49*(4), 733-756.

Schmidt, R. (1990). The role of consciousness in second language learning. *Applied Linguistics*, *11*(2), 129-158.

Symons, C. S., & Johnson, B. T. (1997). The self-reference effect in memory: A meta-analysis. *Psychological Bulletin*, *121*(3), 371-394.

Thomson, R. I. (2011). Computer assisted pronunciation training: Targeting second language vowel perception improves pronunciation. *CALICO Journal*, *28*(3), 744-765.

Thomson, R. I. (2012). Improving L2 listeners' perception of English vowels: A computer-mediated approach. *Language Learning*, *62*(4), 1231-1258.

Thomson, R. I., & Derwing, T. M. (2015). The effectiveness of L2 pronunciation instruction: A narrative review. *Applied Linguistics*, *36*(3), 326-344.

van den Oord, A., Dieleman, S., Zen, H., Simonyan, K., Vinyals, O., Graves, A., Kalchbrenner, N., Senior, A., & Kavukcuoglu, K. (2016). WaveNet: A generative model for raw audio. *arXiv preprint arXiv:1609.03499*.

Wang, C., Chen, S., Wu, Y., Zhang, Z., Zhou, L., Liu, S., Chen, Z., Liu, Y., Wang, H., Li, J., He, L., Zhao, S., & Wei, F. (2023). Neural codec language models are zero-shot text to speech synthesizers. *arXiv preprint arXiv:2301.02111*.

Werker, J. F., & Tees, R. C. (1984). Cross-language speech perception: Evidence for perceptual reorganization during the first year of life. *Infant Behavior and Development*, *7*(1), 49-63.

Winner, L. (1980). Do artifacts have politics? *Daedalus*, *109*(1), 121-136.

Witt, S. M., & Young, S. J. (2000). Phone-level pronunciation scoring and assessment for interactive language learning. *Speech Communication*, *30*(2-3), 95-108.

Zechner, K., Evanini, K., Ramanarayanan, V., & Wang, X. (2019). Automated scoring of speaking tasks in the Test of English-for-Teaching. *ETS Research Report Series*, *2019*(1), 1-13.

---

*Discussion Questions*

1. How would a pronunciation AI system designed around Jenkins' Lingua Franca Core differ in its feedback from current commercial tools? What phonological features would it assess, and which would it ignore?

2. Consider the SLM-r's prediction that perceptual category formation precedes productive mastery. What implications does this have for the design of AI pronunciation training sequences? Should AI tools spend more time on listening discrimination and less on production practice?

3. A learner of English from Nigeria receives consistently low scores from an AI pronunciation app calibrated to General American English norms. The learner's speech is highly intelligible to diverse interlocutors. How should a teacher address this situation? What role should the AI tool play, if any, going forward?

4. Voice cloning technology can generate speech in a learner's own voice with target-like pronunciation. What are the potential benefits and risks of using this technology in pronunciation instruction? How might it interact with learner identity and investment?

5. Design a pronunciation teaching unit for a specific L1-L2 pairing (e.g., Mandarin L1 learners of English) that integrates AI tools according to the six principles outlined in Section 10.8.1. What would each session include, and how would AI and human instruction be sequenced?
