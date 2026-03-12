# Domain Pitfalls: Geriatric Rehabilitation Protocols

**Domain:** Evidence-Based Geriatric Physical Therapy / Rehabilitation Protocols
**Researched:** 2026-03-12
**Confidence note:** Web search and WebFetch tools were unavailable during this research session. All findings are drawn from training knowledge covering published clinical literature, RCTs, systematic reviews, and major guideline bodies (AGS, IASP, WHO, ACSM, APTA) up to August 2025. Confidence is rated MEDIUM across the board — claims reflect established clinical consensus, but live verification against current guidelines is recommended before each comorbidity phase begins.

---

## Critical Pitfalls

Mistakes in this category cause protocol rewrites, patient harm, or fundamental invalidation of the evidence base.

---

### Pitfall 1: Applying Adult Dosage Directly to Elderly Populations (Age-Agnostic Prescription)

**What goes wrong:** RCT evidence for exercise dosage (intensity, frequency, volume) is often derived from mixed-age adult populations, with elderly subjects underrepresented or analyzed as a subgroup only in post-hoc analysis. Copying the headline dosage (e.g., "3 sets x 15 reps at 70% 1RM for knee OA") into a geriatric protocol without adjustment produces a protocol that is physiologically mismatched to the target population.

**Why it happens:** Systematic reviews pool heterogeneous studies; their forest plots and summary recommendations represent average effects across a broad age range. Researchers building on these reviews often read the abstract conclusion, not the population characteristics table. The default is to trust the headline finding.

**Consequences:**
- Acute injury from overloading sarcopenic or osteoporotic musculature
- Early dropout from perceived excessive difficulty, creating a data trail that makes the protocol look ineffective
- Autonomic overload in patients with compromised cardiac reserve (particularly relevant for DPOC, Insuficiência Cardíaca, Parkinson protocols)
- Fracture risk in osteoporotic patients placed under high-impact loads without prior bone mineral density confirmation

**Prevention:**
- For every dosage parameter cited, trace the original study and record the mean age and frailty status of subjects
- Apply the "Start low, go slow, but reach the goal" principle (already in PROJECT.md) as a non-negotiable constraint, not a stylistic preference
- Use accepted geriatric intensity anchors: RPE (Borg 6-20 scale) 11-13 in Acute phase, 13-15 in Subacute, 15-17 maximum in Advanced — always alongside absolute cutoffs
- Cross-reference ACSM's Exercise Guidelines for Older Adults (current edition) for population-specific dosage ranges

**Detection (warning signs):**
- Protocol cites a dosage without specifying the mean age or frailty level of the source study
- Intensity is described only in % of 1RM without RPE equivalent
- No phase-specific upper limits on volume

**Phase mapping:** Affects every comorbidity from Protocol 1 (Osteoartrite) onward. Highest risk in Protocols 5 (Fratura de Femur), 6 (Parkinson), 8 (Sarcopenia), 16 (Insuficiência Cardíaca).

---

### Pitfall 2: Treating Frailty as Binary (Frail vs. Not Frail) Instead of a Spectrum

**What goes wrong:** Protocols written without frailty stratification implicitly assume a homogeneous patient. In reality, a "geriatric" patient may be robust, pre-frail, or frail (Fried Phenotype) or may score 3-7 on the Clinical Frailty Scale (CFS). The same exercise dose that is therapeutic for a robust 78-year-old is dangerous for a pre-frail 74-year-old with weight loss and slow gait speed.

**Why it happens:** Frailty assessment tools (Fried Phenotype, CFS, FRAIL scale) are well-validated but add clinical time. Protocol writers under time pressure assume the treating clinician will "adjust as needed," leaving no structured guidance for that adjustment.

**Consequences:**
- Robust elderly patients are under-challenged and fail to achieve meaningful functional gains
- Frail patients are over-challenged, leading to falls, fatigue, and post-exercise delirium (particularly in dementia patients)
- Protocol cannot be audited or reproduced because the key moderating variable (frailty) is undefined

**Prevention:**
- Include frailty screening (Fried Phenotype or CFS) as a mandatory baseline assessment alongside TUG, SPPB, and Manual Dynamometry
- Provide frailty-stratified dosage tables within each protocol: one column for Robust, one for Pre-frail, one for Frail
- Set explicit phase-advancement criteria tied to frailty score (e.g., advance from Acute to Subacute only when CFS ≤ 4 AND TUG < 20s)

**Detection:**
- Protocol does not mention frailty screening tool by name
- Dosage is presented as a single fixed value with no stratification
- Phase advancement criteria are time-based only ("after 4 weeks") rather than performance-based

**Phase mapping:** Protocols 5, 7, 8, 18, 19 are highest risk (hip fracture, falls, sarcopenia, dementia, vertebral fractures). Frailty stratification should be designed in Protocol 1 as the template for all subsequent comorbidities.

---

### Pitfall 3: Ignoring Polypharmacy Interactions with Exercise Physiology

**What goes wrong:** Elderly patients averaging 5-10 medications have drug-exercise interactions that alter the safety and efficacy of the protocol. The most dangerous classes are: antihypertensives (blunted heart rate response, orthostatic hypotension risk), beta-blockers (RPE-based intensity monitoring invalidated if not corrected), diuretics (exercise-induced dehydration and hypokalemia), anticoagulants (fall risk implications), benzodiazepines/sedatives (proprioception and balance impairment), and anticholinergics (heat intolerance, urinary retention).

**Why it happens:** Physical therapy evidence is generally siloed from pharmacology. RCTs typically exclude polypharmacy patients or do not report medication status in detail. Protocol writers draw from these clean-population studies and produce documents that are contraindicated for a typical geriatric outpatient.

**Consequences:**
- Patient on beta-blocker performs "moderate intensity" exercise that is actually near-maximal for them (RPE miscalibrated without heart rate adjustment)
- Orthostatic hypotension event during balance or gait training in patient on ACE inhibitor + diuretic + alpha-blocker
- Anticoagulated patient (warfarin, rivaroxaban) falls during balance exercise without the protocol having documented fall-event protocol or bruise/hematoma monitoring

**Prevention:**
- Each protocol must include a "Polypharmacy Interaction" section listing the most common drug classes for that comorbidity and their specific exercise implications
- For patients on beta-blockers: replace HR-based intensity with Talk Test or RPE (Borg); note the correction factor
- For patients on antihypertensives/diuretics: mandate pre- and post-exercise blood pressure check; define BP cut-offs for stopping exercise (e.g., systolic > 180 mmHg at rest = defer session)
- For patients on anticoagulants: document fall-event protocol (ice, compression, medical notification within X minutes)
- Reference AGS Beers Criteria (2023 update) for high-risk medication flags in geriatric patients

**Detection:**
- Protocol mentions exercise intensity without noting beta-blocker confound
- No pre-session vital signs protocol
- No fall-event response protocol for patients on anticoagulants or osteoporosis drugs

**Phase mapping:** Universal, but specifically critical for Protocols 16 (Insuficiência Cardíaca — beta-blockers, diuretics), 15 (DPOC — bronchodilators, corticosteroids), 6 (Parkinson — levodopa timing relative to exercise sessions), 17 (Neuropatia Diabética — hypoglycemia risk during exercise).

---

### Pitfall 4: Underestimating Fall Risk During Therapeutic Exercise (Exercise-Induced Fall)

**What goes wrong:** Falls are both a comorbidity treated by geriatric rehab and a risk created by geriatric rehab. Balance and gait training — the core interventions for protocols 7 (Quedas), 6 (Parkinson), 3 (AVC), and 8 (Sarcopenia) — require the patient to operate at or near their stability limits. A protocol that does not formally risk-stratify for exercise-induced falls and provide structured mitigation creates liability and harm.

**Why it happens:** Fall risk is assessed at admission (TUG, SPPB, Berg Balance Scale), then the protocol moves to intervention. The risk assessment is treated as a baseline snapshot rather than a dynamic parameter to be reassessed during each session. Post-exercise fatigue, which substantially increases fall risk in the 2-4 hours after a session, is rarely addressed.

**Consequences:**
- Intra-session fall during unsupported stance or dual-task walking exercise
- Post-session fall during ambulation to exit the clinic (post-exercise fatigue + hypotension)
- Fear of falling (kinesiophobia) triggered by near-fall during session, causing dropout

**Prevention:**
- Include session-level fall risk protocol: pre-session assessment of fatigue level (VAS), medication timing, orthostatic BP check
- Mandate use of gait belt or spotter criteria by TUG score (e.g., TUG > 20s = gait belt mandatory)
- Define supervised vs. unsupported exercise criteria
- Include post-session cool-down and supervised ambulation-to-exit protocol
- Reassess TUG and Berg at every phase transition, not only at admission

**Detection:**
- Protocol describes balance exercises without specifying equipment (parallel bars, gait belt, spotter)
- No post-session monitoring protocol
- Fall risk assessment is listed only at baseline, not during phase progression

**Phase mapping:** Protocols 7 (primary), 6, 3, 8 are highest risk. Also relevant in Protocol 5 (hip fracture — fear of re-fracture) and 19 (vertebral fractures — fear of new compression).

---

### Pitfall 5: Ignoring Cognitive Barriers to Protocol Compliance and Learning

**What goes wrong:** Protocols assume the patient can understand multi-step exercise instructions, remember the home exercise program (HEP), self-monitor effort, and report symptoms accurately. Mild Cognitive Impairment (MCI) or early dementia — highly prevalent in patients aged 75+ — fundamentally alters all four of these assumptions. The result is a protocol that is theoretically valid but practically impossible for the actual patient population to follow.

**Why it happens:** Cognitive screening is absent from most geriatric rehabilitation research protocols (RCTs routinely exclude MMSE < 24 patients, then practitioners apply findings to patients who would have been excluded). The protocol writer inherits this exclusion bias without flagging it.

**Consequences:**
- Patient cannot follow 3-step exercise instruction; therapist improvises in-session but HEP compliance is zero
- Incorrect self-reported RPE (patients with dementia tend to underreport exertion)
- Adverse events unreported (patient does not recognize or communicate pain change)
- Care partner burden ignored: HEP requires caregiver execution, but protocol says nothing about caregiver training

**Prevention:**
- Mandate cognitive screening at baseline: MMSE or MoCA (MoCA is more sensitive for MCI); document score in protocol intake
- Stratify instruction complexity: for MMSE < 24, limit HEP to 2-3 exercises maximum, use visual/pictographic instruction sheets, require caregiver to observe at least one session
- For Protocol 18 (Demência/Alzheimer): design all exercises as procedural (implicit) learning tasks (repetitive, routine-based, non-declarative) rather than instructional learning
- Use observational pain scales (PAINAD, Abbey Pain Scale) alongside or instead of VAS for patients with moderate-to-severe dementia
- Include caregiver training as a formal protocol component, not an afterthought

**Detection:**
- Protocol instructions use multi-step verbal cues without visual alternatives
- HEP is described with 5+ exercises
- No mention of cognitive screening tool
- Pain assessment uses only patient self-report

**Phase mapping:** Protocol 18 (Demência/Alzheimer) — primary. Also critical for Protocol 6 (Parkinson — executive dysfunction), Protocol 3 (AVC — aphasia, apraxia), Protocol 7 (Quedas — fear/anxiety interaction).

---

## Moderate Pitfalls

Mistakes here degrade protocol quality, reduce efficacy, or create reproducibility problems, but do not immediately cause patient harm.

---

### Pitfall 6: Evidence Pooling Across Clinically Heterogeneous Subgroups

**What goes wrong:** "Osteoarthritis" in a meta-analysis may pool hip OA, knee OA, hand OA, and spinal OA. "Chronic low back pain" pools specific (stenosis, spondylolisthesis) and non-specific etiologies. If a protocol cites evidence from a pooled review and then prescribes it for a specific subtype, the recommendation may be founded on data that is largely irrelevant to the target patient.

**Why it happens:** Systematic reviews are cited by title/topic, not by population subgroup analyzed. High-impact journals favor broad inclusion for statistical power. Protocol writers follow the citation rather than auditing the population.

**Prevention:**
- For each protocol, explicitly state the ICD-10/clinical definition of the target population
- When citing a meta-analysis, note: mean age, OA joint site, comorbidity inclusion/exclusion criteria, and primary outcome measured
- Flag whenever the cited study population meaningfully differs from the target population (e.g., "This RCT excluded patients with TUG > 15s — extrapolation to severe geriatric frailty is limited")

**Detection:**
- Protocol references a review on "osteoarthritis" without specifying joint or severity subgroup
- Age range of cited studies is not reported

**Phase mapping:** Protocols 1 (Osteoartrite), 2/12 (Lombalgia), 9 (Espondilose), 20 (Gonalgia/Coxalgia) — all conditions where clinical heterogeneity within the diagnosis label is high.

---

### Pitfall 7: Prescribing Absolute Rest Periods Instead of Active Recovery

**What goes wrong:** Older protocols (pre-2010) recommended rest between exercise phases. More recent evidence strongly supports active recovery (light movement, breathing exercises, seated walking) over passive rest in geriatric populations. Protocols that still prescribe "rest 2 minutes between sets" miss an opportunity to maintain circulation, reduce post-exercise stiffness, and prevent orthostatic drop.

**Why it happens:** Older evidence base and professional inertia. Many training programs teach passive rest as the standard.

**Prevention:**
- Replace "rest X minutes" with "active recovery: gentle walking or seated marching for X minutes"
- Reference current ACSM Older Adult guidelines on inter-set recovery strategies

**Detection:**
- Protocol says "rest between sets" without specifying type of rest
- No mention of cardiovascular response during rest periods

**Phase mapping:** Protocols 15 (DPOC), 16 (Insuficiência Cardíaca), 8 (Sarcopenia) — where inter-set recovery strategy directly impacts session safety.

---

### Pitfall 8: Single-Dimension Outcome Measurement (Missing Functional Composites)

**What goes wrong:** A protocol defines success as improvement in a single metric (e.g., VAS pain score, or grip strength in kg). In geriatric populations, meaningful recovery is multidimensional: pain, strength, balance, functional mobility, fear of movement, and quality of life all move semi-independently. A protocol focused on one metric can show "success" on paper while the patient declines functionally.

**Why it happens:** Single metrics are easier to measure, power calculations in RCTs favor single primary outcomes, and protocol writers mimic the research structure.

**Prevention:**
- Mandate a minimum outcome battery at each phase transition: TUG (mobility), SPPB (functional composite), Manual Dynamometry (strength), pain VAS/NRS, and one condition-specific scale (e.g., WOMAC for OA, MDS-UPDRS for Parkinson)
- This is already required by PROJECT.md for TUG, SPPB, Dynamometry — the pitfall is omitting condition-specific instruments or patient-reported outcomes

**Detection:**
- Protocol lists outcome measures only at admission and discharge, not at phase transitions
- No patient-reported outcome measure (PROM) included

**Phase mapping:** Universal. Template established in Protocol 1.

---

### Pitfall 9: Ignoring Pain Sensitization and Central Sensitization in Chronic Conditions

**What goes wrong:** For chronic pain conditions (Lombalgia Crônica, Gonalgia/Coxalgia degenerativa, Artrose), protocols often operate on a purely biomechanical model: strengthen muscles, reduce joint stress, pain resolves. In elderly patients with long-standing chronic pain, central sensitization is frequently present — the nervous system has upregulated pain signaling independent of peripheral tissue state. Exercise will not resolve central sensitization on its own, and pain-contingent exercise titration (stopping when pain appears) may reinforce sensitization.

**Why it happens:** Biomechanical models are more intuitive for physical therapists. Central sensitization assessment tools (CSI, PainDETECT) are underused in geriatric rehab.

**Prevention:**
- Screen for central sensitization features at baseline in all chronic pain protocols: widespread pain, allodynia, fatigue, sleep disturbance, catastrophizing (PCS)
- Use time-contingent rather than pain-contingent exercise progression for patients with central sensitization features
- Include brief pain education component (Explain Pain / Pain Neuroscience Education) adapted for cognitive level
- Reference IASP guidelines on chronic pain in older adults (directly mandated by PROJECT.md)

**Detection:**
- Protocol uses pain VAS as the sole exercise progression criterion ("stop if pain > 4/10")
- No mention of pain catastrophizing or central sensitization screening
- No pain education component

**Phase mapping:** Protocols 2, 12 (Lombalgia), 1 (Osteoartrite), 20 (Gonalgia/Coxalgia), 13 (Ombro Doloroso), 9 (Espondilose).

---

### Pitfall 10: Underaddressing Respiratory and Cardiovascular Precautions in Non-Cardiopulmonary Protocols

**What goes wrong:** A protocol for knee OA or hip fracture rehabilitation does not formally address cardiovascular precautions because the condition is "musculoskeletal." But the geriatric patient with knee OA typically has 2-4 additional comorbidities, and cardiovascular/pulmonary reserve limitations are the most common exercise limiters in patients aged 70+. A protocol that ignores this produces an intensity recommendation that is structurally valid but physiologically dangerous.

**Why it happens:** Protocols are organized by primary diagnosis. Cross-system precautions are considered the responsibility of medical clearance, not the protocol document.

**Prevention:**
- Every protocol must include a "Cardiorespiratory Precautions" section regardless of primary diagnosis
- Mandate pre-session vital signs (HR, BP, SpO2) for all patients aged 70+ or with any documented cardiovascular or pulmonary comorbidity
- Define absolute and relative contraindications to starting/continuing a session: e.g., resting SpO2 < 90%, resting HR > 100 bpm, systolic BP > 180 mmHg
- Reference AHA/ACC and ACSM exercise preparticipation screening guidelines for older adults

**Detection:**
- Protocol has no vital signs monitoring requirement
- No session suspension criteria listed
- "Cardiovascular precautions" delegated only to physician medical clearance with no session-level protocol

**Phase mapping:** Highest urgency in Protocols 16 (Insuficiência Cardíaca) and 15 (DPOC), but must be present as a standard section in every protocol.

---

### Pitfall 11: Home Exercise Program (HEP) Design Detached from Real-World Adherence Data

**What goes wrong:** HEP is designed by a clinician who knows the exercises are beneficial, then handed to the patient with no structure for overcoming the actual barriers to adherence: fatigue, pain, environmental constraints, social isolation, lack of supervision, and competing health priorities. Geriatric HEP adherence rates in published studies average 40-60%, meaning the protocol's efficacy depends on half the prescribed dose actually being delivered.

**Why it happens:** HEP is treated as a clinical prescription, not a behavior change challenge. The research that shows benefit usually occurs in supervised settings; HEP components are added based on theoretical extrapolation.

**Prevention:**
- Design HEP with adherence barriers explicitly addressed: provide equipment-free alternatives, seated alternatives for low-energy days, visual instruction sheets
- Include a brief self-monitoring tool: simple checklist the patient or caregiver marks after each session
- Specify what to do when a session is missed (do not double-dose; resume normally)
- Consider telehealth or phone check-in touchpoints between in-person sessions as adherence support — flag this as protocol-adjacent infrastructure
- Reference motivational interviewing techniques for exercise adherence in older adults (well-supported in AGS position statements)

**Detection:**
- HEP is a list of exercises only, with no adherence structure
- No mention of what happens if patient misses sessions
- HEP requires equipment not available in typical home environment

**Phase mapping:** Universal, but especially critical for Protocols 7 (Quedas — high HEP importance for independence), 4 (Osteoporose — long-term loading for bone remodeling requires sustained HEP adherence).

---

### Pitfall 12: Comorbidity Interaction Blindness — Treating Diagnoses in Isolation

**What goes wrong:** A patient presenting for Protocol 10 (ATJ — Post-op Total Knee Arthroplasty) may simultaneously have Parkinson's disease, peripheral neuropathy, and cardiac insufficiency. The ATJ protocol designed for an otherwise healthy older adult is contraindicated without modification. Treating each diagnosis as a standalone entity produces protocols that are internally valid but externally irrelevant for most actual patients.

**Why it happens:** RCTs and clinical guidelines are organized by single diagnosis. Cross-comorbidity interaction guidance is sparse in the literature.

**Prevention:**
- Each protocol must include a "Comorbidity Interaction" section listing the 3-5 most common concurrent diagnoses and how they modify the protocol
- Use the project's own 20-comorbidity list as a cross-reference matrix: for Protocol 10 (ATJ), cross-reference Protocols 6, 17, and 16 for modification guidance
- Flag when a comorbidity combination represents a relative or absolute contraindication to a specific modality (e.g., TENS is a relative contraindication in patients with cardiac pacemakers — relevant to multiple protocols)

**Detection:**
- Protocol contains no comorbidity interaction section
- Protocol assumes single-diagnosis patient (exclusion criteria not stated)

**Phase mapping:** Highest risk for Protocols 5 (Fratura Femur — often occurs in already frail, multimorbid patients), 10 and 11 (post-arthroplasty — older patients commonly have cardiac and metabolic comorbidities), 18 (Demência — cognitive impairment interacts with every other protocol).

---

## Minor Pitfalls

---

### Pitfall 13: Levodopa Timing Ignored in Parkinson Protocol

**What goes wrong:** Exercise performance and safety in Parkinson's disease patients depends critically on the timing of levodopa administration relative to the therapy session. Exercise during "off" periods (low dopamine) markedly increases freezing risk, dyskinesia burden, and fall risk. Protocols that do not specify session timing relative to medication schedule are clinically incomplete.

**Prevention:** Protocol 6 must include a levodopa timing recommendation: schedule sessions 45-60 minutes after medication dose (peak "on" state). Communicate timing requirement to patient's neurologist.

**Phase mapping:** Protocol 6 (Parkinson) only, but serves as template for other pharmacotherapy-sensitive protocols.

---

### Pitfall 14: Ignoring Sex and Hormonal Differences in Musculoskeletal Protocols

**What goes wrong:** Osteoporosis, pelvic floor dysfunction, and hip fracture have dramatically different prevalence, presentation, and exercise response by sex. Post-menopausal estrogen loss affects bone remodeling rate, proprioception, and joint laxity in ways that modify exercise prescription. Protocols using sex-aggregated data may systematically under-serve or over-challenge one group.

**Prevention:** Note sex-specific prevalence and evidence gaps in each relevant protocol. For Protocol 4 (Osteoporose) and Protocol 14 (Assoalho Pélvico), specify sex-differentiated outcome targets where evidence supports it.

**Phase mapping:** Protocols 4, 5, 14, 13, 19.

---

### Pitfall 15: Neglecting Thermoregulatory Impairment in Exercise Intensity Guidance

**What goes wrong:** Elderly patients have reduced thermoregulatory capacity (decreased sweating rate, reduced cardiovascular response to heat, blunted thirst sensation). Exercise environments and high-intensity sessions carry real hyperthermia risk that adult-population protocols do not address. This is especially relevant for DPOC and cardiac patients.

**Prevention:** Include clinic environment temperature guidance (< 24°C preferred), hydration reminders, and early warning signs of heat intolerance in Acute phase protocols.

**Phase mapping:** Protocols 15 (DPOC), 16 (Insuficiência Cardíaca), 8 (Sarcopenia — high muscle mass deficiency reduces heat dissipation).

---

### Pitfall 16: Failing to Specify Outcome Measure Minimal Clinically Important Differences (MCIDs)

**What goes wrong:** A protocol requires TUG improvement but does not specify what change constitutes meaningful improvement (MCID for TUG is approximately 3.5 seconds in older adults). Without MCID anchors, phase advancement decisions are arbitrary and the protocol cannot be audited for clinical relevance.

**Prevention:** Document MCID values for each outcome measure used in the protocol. Published MCIDs for geriatric population: TUG ~3.5s, SPPB ~0.5 points (some sources ~1 point), grip strength ~5 kg, WOMAC ~9.7 points (pain subscale).

**Phase mapping:** Universal — establish in Protocol 1 template.

---

## Evidence Synthesis Pitfalls

These affect the research process that feeds into protocol creation, not the protocol itself.

---

### Pitfall E1: Confusing Guideline Grade with Evidence Quality

**What goes wrong:** A "Grade A" recommendation in a clinical guideline is a statement about the consistency of the evidence base, not necessarily the quality of individual studies. Some Grade A recommendations are founded on multiple low-quality consistent studies. Treating "Grade A" as equivalent to "high-quality RCT evidence" inflates confidence in certain recommendations.

**Prevention:** When citing a guideline recommendation, always locate and assess the underlying evidence table. Note the number and quality of supporting studies, not just the grade letter.

**Detection:** Protocol says "Level A evidence (AGS 2019)" without citing the underlying RCTs.

---

### Pitfall E2: Recency Bias — Assuming Newer Study Supersedes Previous Systematic Review

**What goes wrong:** A new RCT (n=60) published in 2024 appears to contradict a 2020 Cochrane review (n=2400 pooled). Protocol writer privileges the newer study because it is more recent. The newer study may be a statistical outlier, use an atypical population, or report on a novel outcome.

**Prevention:** Weight evidence by study hierarchy and sample size, not publication date. Use the 2024 RCT to note "emerging evidence" if it contradicts established reviews, but do not replace the systematic review recommendation.

---

### Pitfall E3: Ignoring Publication Bias in Exercise Research

**What goes wrong:** Positive results from exercise interventions are dramatically more likely to be published than null results in geriatric rehabilitation literature. Exercise is also subject to "allegiance bias" (researchers who believe in exercise publish more favorable results). Meta-analyses of published studies inherit this bias, potentially inflating effect sizes.

**Prevention:** Check for Cochrane reviews with funnel plot analysis. Look for grey literature and registered trials with null results. Explicitly state when evidence base is likely affected by publication bias (e.g., balance training for falls prevention — large positive literature but significant publication bias documented).

---

## Phase-Specific Warnings by Comorbidity

| Protocol | Comorbidity | Top Pitfall Risk | Key Mitigation |
|----------|-------------|-----------------|----------------|
| 1 | Osteoartrite | Evidence heterogeneity (joint site pooling); central sensitization ignored | Specify joint/severity subgroup in all citations; include PCS screening |
| 2/12 | Lombalgia Crônica | Central sensitization treated as biomechanical; pain-contingent dosing | Time-contingent progression; PNE component |
| 3 | AVC (fase crônica) | Cognitive/aphasia barriers; neuroplasticity window assumptions | Implicit learning approaches; caregiver training |
| 4 | Osteoporose | Impact loading contraindicated without BMD data; HEP adherence for long-term remodeling | DXA result review; behavioral adherence support |
| 5 | Fratura de Femur/Quadril | Frailty underestimation; post-op fear of movement | CFS at admission; kinesiophobia screening (Tampa Scale) |
| 6 | Parkinson | Levodopa timing ignored; cognitive-executive barriers to learning | Schedule sessions post-dose; procedural learning tasks |
| 7 | Quedas/Pós-Queda | Exercise-induced falls during protocol; post-exercise fall window | Gait belt criteria; post-session supervised exit |
| 8 | Sarcopenia | Adult dosage applied; protein intake not coordinated | Geriatric-specific load ranges; dietitian referral pathway |
| 9 | Espondilose | Stenosis severity not stratified; lumbar flexion vs. extension evidence confusion | Classify by stenosis grade; differentiate neurogenic claudication management |
| 10 | ATJ Pós-op | DVT/PE risk window; cardiac comorbidity interaction | VTE prophylaxis protocol awareness; cardiorespiratory precautions |
| 11 | ATQ Pós-op | Hip precaution violations during functional exercises; surgeon protocol conflicts | Specify precaution set (posterior vs. anterior approach); surgeon coordination |
| 12 | Lombalgia Inespecífica | Same as Protocol 2; overmedicalizing a condition that benefits from active coping | Avoid passive modality overreliance; education-forward approach |
| 13 | Ombro Doloroso | Rotator cuff tear underdetected; glenohumeral instability loaded prematurely | Imaging review required before high-load prescription |
| 14 | Assoalho Pélvico | Pelvic floor overactivity treated identically to underactivity | Functional assessment to determine hyper vs. hypo tone before exercise type selection |
| 15 | DPOC | SpO2 monitoring absent; over-ambitious aerobic targets | Mandatory SpO2 monitoring; Borg CR10 dyspnea scale |
| 16 | Insuficiência Cardíaca | Beta-blocker confound; fluid retention masking exercise response | RPE-only intensity; daily weight monitoring coordination with cardiology |
| 17 | Neuropatia Diabética | Hypoglycemia during exercise; proprioceptive deficit depth underestimated | Pre-session glucose check; sensory-loss-adapted balance exercises |
| 18 | Demência/Alzheimer | Declarative learning assumed; caregiver burden ignored | Procedural/routine-based tasks only; mandatory caregiver training component |
| 19 | Fraturas Vertebrais | Flexion exercises prescribed before osteoporosis protocol | No end-range spinal flexion in osteoporotic patients; extension-based loading |
| 20 | Gonalgia/Coxalgia | Same as Protocol 1 but with higher chronicity burden; central sensitization more likely | CSI screening; pain education component elevated in priority |

---

## Cross-Cutting Structural Pitfalls (Protocol Design)

### Pitfall S1: Protocol Template Rigidity — Forcing 3-Phase Model on All Conditions

**What goes wrong:** If the project establishes a 3-phase Acute/Subacute/Advanced template in Protocol 1 and applies it mechanically to all 20 comorbidities, conditions with different clinical timelines get distorted. Post-op ATJ and ATQ have well-defined surgical phase constraints. Chronic conditions (Lombalgia Crônica Inespecífica) do not have an "Acute" phase in the same sense. Stroke rehabilitation in the chronic phase is not organized around injury timeline at all.

**Prevention:** PROJECT.md already specifies flexible phase count (2-4) — this pitfall is about not honoring that flexibility. For each comorbidity, derive the phase structure from the clinical literature for that condition, not from the Protocol 1 template.

**Phase mapping:** Most relevant for Protocols 2, 3, 12, 18 where the standard acute/recovery model does not map cleanly.

---

### Pitfall S2: Losing "Start Low, Go Slow, But Reach the Goal" in the Subacute Phase

**What goes wrong:** Protocols successfully implement conservative Acute phase prescriptions, then overcompensate in the Subacute phase with an abrupt intensity jump that violates the progressive overload principle adapted for geriatric patients. The "reach the goal" part of the principle is emphasized; the progressive path to get there is underspecified.

**Prevention:** Define explicit week-by-week or session-by-session progression targets in the Subacute phase, not just start and end points. Specify the maximum allowable progression rate (e.g., "no more than 10% increase in load per week" per ACSM guidelines for older adults).

---

### Pitfall S3: Outcome Measures Not Translated/Validated in Brazilian Portuguese

**What goes wrong:** Several standard geriatric assessment tools have Portuguese-Brazilian validated versions that differ from European Portuguese or Spanish-Portuguese translations. Using the wrong version introduces measurement error and prevents valid comparison with Brazilian clinical literature.

**Prevention:** For each outcome measure, verify the Brazilian Portuguese version specifically: WOMAC-BR, SPPB (validated in Brazil by Nakano 2007), MoCA-BR, SF-36 Brazil, PDQ-39 Brazil. Cite the Brazilian validation study for each tool.

**Phase mapping:** Universal, but most critical at Protocol 1 as template-setter.

---

## Sources

**Confidence note:** All sources listed below are from training knowledge (knowledge cutoff August 2025). Web verification was unavailable during this research session. All citations should be independently verified before clinical application.

**Key guideline bodies and documents (MEDIUM confidence — established, stable sources):**
- American Geriatrics Society (AGS) Clinical Practice Guidelines, including Beers Criteria 2023 update
- IASP Guidelines on Chronic Pain in Older Persons
- WHO Global Action Plan on Physical Activity 2018-2030 (older adult components)
- ACSM's Exercise Guidelines for Older Adults (current edition — verify current edition number)
- AHA/ACC Exercise Preparticipation Health Screening Guidelines

**Key research areas (MEDIUM confidence — consensus across multiple RCTs and systematic reviews as of training cutoff):**
- Fried Phenotype (Fried et al., 2001 — foundational, stable)
- Clinical Frailty Scale (Rockwood et al. — validated, widely adopted)
- SPPB validation in Brazil (Nakano et al., 2007)
- Levodopa-exercise timing in Parkinson's (multiple RCTs, consistent finding)
- Central Sensitization Inventory (Mayer et al., 2012)
- Pain Neuroscience Education in chronic musculoskeletal pain (Louw et al., systematic reviews)
- TUG MCID in geriatric population (Bohannon, multiple validation studies)
- AGS Beers Criteria — specifically relevant for polypharmacy exercise interactions
- MoCA sensitivity for MCI detection vs. MMSE (Nasreddine et al., multiple validation replications)

**Gaps requiring live verification (LOW confidence — need current source confirmation):**
- Current ACSM Older Adult Guidelines edition and specific dosage tables
- Most recent Cochrane reviews for specific comorbidities (osteoarthritis, DPOC, heart failure exercise)
- Current AGS frailty management position statement
- Brazilian Portuguese validation status of all 20+ outcome measures used across protocols
