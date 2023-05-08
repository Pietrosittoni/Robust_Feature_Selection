# Robust_Feature_Selection

The goal of this project is to define a stable feature selection method for identifying a subset of the most relevant features/questions to use in a binary classification problem that involves determining who answered a questionnaire honestly and who did not.

The theme of the questionnaire, the number of items/features, and the number of participants differ for each dataset, but the binary response variable is the same for all datasets.

All available responses were in multiple choice format, with participants only having the option of selecting one option for each questionnaire item.The experiment consisted in answering the questions one time in the most honest way possible and the second time according to a scenario in which they were instructed to lie.
Each participant was required to respond estimating his/her agreement using a 5-point Likert scale (where 1 indicates a strong disagreement and 5 a strong agreement), except for a dataset where the scale goes from 4 to 20. 


****
1)SD3 (Short Dark Triad 3)
* Type: Dark Triad
* Number of Items: 27 (Machiavellism, Narcissism, Psychopathy)
* Participants:
  * CC: 241
  * JI: 432
* JI: participants were told that they were going through a job interview (JI) that they cared a lot for, and they had to complete a questionnaire trying to avoid showing undesirable personality traits, putting themselves "under the better light possible."
* CC: participants received the instructions of completing a personality questionnaire imagining to be a parent that was undergoing a cause for the custody of his/her children (CC), and therefore, they had to show to be a good parent.
* FAKING GOOD: we expect liars will give lower responses than truth-tellers because they have to minimize negative traits
****
2)PMRQ (Questionnaire on prospective and retrospective memory)
* Type: Memory
* Number of Items: 16
* Participants: 
  *	702
* Subjects were asked to respond twice to a test developed to identify specific memory difficulties, following different instructions: the first time answering honestly, and the second time faking a memory deficit.
* FAKING BAD: we expect liars will give higher responses than truth-tellers because they have to exaggerate memory symptoms
****
3)PCL (Posttraumatic Stress Disorder Checklist for DSM-5)
* Type: Post Traumatic Stress Disorder (PTSD)
* Number of Items: 20
* Participants: 
  * 201
* It was asked to participants to answer twice a questionnaire developed to identify possible victims of PTSD, following different instructions: the first time by answering honestly, while the second time pretending to be victims of Post Traumatic Stress Disorder. 
* FAKING BAD: we expect liars will give higher responses than truth-tellers because they have to exaggerate PTSD symptoms.
****
4)NAQ-R (Negative Acts Questionnaire–Revised)
* Type: Mobbing
* Number of Items: 22
* Participants: 
  * 356
* It was asked to subjects to answer twice a questionnaire developed to identify possible victims of mobbing following different instructions: the first time by answering honestly, while the second time by pretending to be victims of mobbing.
* FAKING BAD: we expect liars will give higher responses than truth-tellers because they have to exaggerate bullying symptoms
****
5)PHQ-9 + GAD-7 (Patient Health Questionnaire + Generalized Anxiety Disorder)
* Type: Anxious-depressive syndrome
* Number of Item: 16 (9+7)
* Participants: 
  * 559
* It was asked to participants to answer twice a questionnaire (composed by 2 questionnaire: PHQ and GAD) developed to identify possible victims of Anxious-depressive syndrome, following different instructions: the first time by answering honestly, while the second time by pretending to be victims of Anxious-depressive syndrome. 
* FAKING BAD: we expect liars will give higher responses than truth-tellers because they have to exaggerate symptoms
****
6)PID_5 (Personality Inventory for DSM-5)
* Type: Mental Disorders 
* Number of Items: 220
* Participants: 
  * 412
* Subjects were asked to answer twice a questionnaire developed to identify mental disorders, following different instructions: the first time by answering honestly, while the second time by pretending to have a mental disorder. 
* FAKING BAD: we expect liars to give higher responses than truth-tellers because they exaggerate mental disorders symptoms.
****
7)shortPID_5 (Personality Inventory for DSM-5) shorter version of PID_5
* Type: Mental Disorders 
* Number of Items: 25
* Participants: 
  * 519
* Subjects were asked to answer twice a questionnaire developed to identify mental disorders, following different instructions: the first time by answering honestly, while the second time by pretending to have a mental disorder.
* FAKING BAD: we expect liars to give higher responses than truth-tellers because they exaggerate mental disorders symptoms.
****
8)PRFQ (Parental Reflective Functioning Questionnaire)
* Type: specific caregivers' ability to mentalize with their children
* Number of Items: 18
* Participants: 
  * 263
* The participants were asked to respond to the final questionnaire twice: the first time honestly, the second time imaging that, as a parent, they were going through a Family Court evaluation and being examined by a psychologist using a test to help determine with whom their children will reside. They were asked to answer test items in such a way as to look like a good parent.
* FAKING GOOD/BAD: depending on the answer we expect liars will give lower or higher responses than truth-tellers because they have to minimize negative traits and emphasize positive traits to appear as a better parent
****
9)IES-R (IMPACT OF EVENTS SCALE-Revised)
* Type: Post Traumatic Stress Disorder (PTSD)
* Number of Item: 22
* Participants: 
  * 179
* It was asked to subjects to answer twice a questionnaire developed to identify possible victims of PTSD, following different instructions: the first time by answering honestly, while the second time pretending to be victims of Post Traumatic Stress Disorder.
* FAKING BAD: we expect liars will give higher responses than truth-tellers because they have to exaggerate PTSD symptoms.
****
10)R_NEO_PI (Revised NEO Personality Inventory)
* Type: Mental Disorders 
* Number of Item: 120
* Participants: 
  * Dishonest: 67176
  * Honest: 10515
* Honest responders have taken the test anonymously with the aim to know themselves and no reason the self deceive themselves. 
Dishonest responders have taken the test in a real job application setting where identity is disclosed. The responders are clearly highly motivated to get the job they applied for.
This is a high stake setting because the respondents do not want to be identified as unreliable responders.
In short, unlike all the fakers in the other datasets, these fake-good responders have not been explicitly instructed to fake but they have set their faking threshold individually.
* FAKING GOOD/BAD: depending on the answer we expect liars will give lower or higher responses than truth-tellers because they have to minimize negative traits and emphasize positive traits
****
11)DDDT (Dark Triad Dirty Dozen)
* Type: Dark Triad
* Number of Items: 12
* Participants: 
  * 492
* Subjects were asked to respond twice to a test developed to identify Dark Triad personality traits, following different instructions: the first time answering honestly, and the second time trying to minimize the Dark Triad personality traits.
* FAKING GOOD: we expect liars will give lower responses than truth-tellers because they have to minimize negative traits
****
12)IADQ (INTERNATIONAL ADJUSTMENT DISORDER QUESTIONNAIRE)
* Type: adjustment disorder
* Number of Items: 9
* Participants: 
  * 225
* Subjects were asked to respond twice to a test developed to identify adjustment disorder, a stress response syndrome defined as a maladaptive behavioural and/or emotional reaction to a psychological stressor that occurs when an individual is unable to properly cope or adjust to a stressful life event.
Subjects firstly had to intentionally fake (bad) their responses, then they had to answer honestly, imagining being in an insurance setting. 
* FAKING BAD: we expect liars to give higher responses than truth-tellers because they try to appear as they have an adjustment disorder to obtain compensation.
****
13)BF
* Type: 5 dimensions of human personality
* Number of Items: 10
* Participants: 
	- CC: 243 (V_df_file)
	- JIS: 221 (CTU_df file)
	- JIHO: 230 (OU_df file)
* Three experiments were conducted where participants were required to respond to the same questionnaire twice. First, they were asked to respond honestly to all of its questions. Then, they were instructed to fake their responses in three different contexts: a Job Interview for a Salesperson Position (JIS), one for a role in a Humanitarian Organization (JIHO) and to obtain a Child Custody (CC) in the context of a litigation, having the same subject responding in an honest condition and in one of instructed faking.
In the three experiments participants were asked to respond to the same set of 10 items twice, first honestly and then altering their answers to obtain a personal gain in three different contexts described before.
* FAKING GOOD: we expect liars will give higher responses than truth-tellers because they have to appear in a better light.
****
