---
permalink: /
title: "Seokchae Yoon"
author_profile: false
classes: page--home
redirect_from:
  - /about/
  - /about.html
---

<section class="hero">
  <img class="hero__photo" src="{{ '/images/profile.jpg' | relative_url }}" alt="Seokchae Yoon">
  <div class="hero__body">
    <h1 class="hero__name">Seokchae Yoon</h1>
    <p class="hero__role">Ph.D. Candidate in Management Engineering (Information Systems Track)<br>KAIST College of Business, Seoul, Korea</p>
    <p>I am advised by Professor Wonseok Oh and expect to complete my degree in 2027. I am on the job market this year.</p>
    <p>My research asks whether the digital and AI services that observe and act on individuals' finances and health genuinely serve those individuals, and what model and deployment design this requires. I build AI models when the question requires one and verify effects with causal inference.</p>
    <p class="chips">
      <a class="chip chip--primary" href="{{ '/files/Seokchae_Yoon_CV.pdf' | relative_url }}">Download CV</a>
      <a class="chip" href="mailto:seokchaeyoon@kaist.ac.kr">Email</a>
      <a class="chip" href="https://scholar.google.com/citations?user=1A6VYAkAAAAJ&hl=ko">Google Scholar</a>
      <a class="chip" href="https://orcid.org/0000-0001-7582-5304">ORCID</a>
      <a class="chip" href="https://github.com/seokchae-yoon">GitHub</a>
    </p>
  </div>
</section>

## Job Market Paper

<div class="card" markdown="1">

**Screening Mental Health with Smartphones: Understanding Real-World Noise in Smartphone-Generated Physiological Data**  
Yoon, S., Oh, J., & Oh, W.  
*Under review at MIS Quarterly.* To be presented at the 2026 Conference on Information Systems and Technology (CIST) and at ICIS 2026.

<details markdown="1">
<summary>Abstract</summary>

Develops a biodynamics-guided deep learning framework for smartphone-based depression screening that quantifies real-world measurement noise through deep-ensemble uncertainty estimation, addressing the reliability problem that limits consumer-grade digital biomarkers.

</details>

</div>

## Research

### Research Themes

<div class="themes">
<div class="theme" markdown="1">

**Healthcare AI**

My dissertation pursues the question in healthcare AI: it builds a noise-robust smartphone-based depression screening model (job market paper, under review at *MIS Quarterly*), causally evaluates a digital therapeutic through randomized trials, and designs hybrid AI underwriting that balances risk protection with access.
{: .theme__text}

<span class="tags">Healthcare IT · Trustworthy AI · Deep Learning</span>
</div>
<div class="theme" markdown="1">

**Platform Economics and Workers**

A second stream, anchored by my publication in *Information Systems Research*, examines how platform services reshape the economic lives of workers, from on-demand wage access to algorithmic matching in ride-hailing.
{: .theme__text}

<span class="tags">Platform Economics · Algorithmic Decision-Making · Causal Inference</span>
</div>
</div>

**Research areas.** Healthcare IT, trustworthy AI and algorithmic decision-making, platform economics.  
**Methods.** Deep learning, causal inference, econometrics, Bayesian statistics and machine learning.

### Dissertation

**When AI Enters the Healthcare Information Environment: Sensing, Treatment, and Markets**  
Committee Chair: Professor Wonseok Oh. Proposal defended May 2026; final defense planned for April 2027.

The dissertation examines what happens when AI relaxes long-standing information constraints in healthcare, across three essays spanning physiological screening, behavioral treatment delivery, and risk-based market design. It argues that the value of AI-generated health information is not fixed, but depends on the reliability of the information the AI produces, the mechanism through which it reaches individuals, and the market structure it enters.

**Essay 1 (Job Market Paper).** Screening Mental Health with Smartphones: Understanding Real-World Noise in Smartphone-Generated Physiological Data. *Under review at MIS Quarterly.*

**Essay 2.** Engaging for Better Sleep: User Interaction and Behavioral Change in a Mobile App-Based Digital Therapeutic for Insomnia. An RCT-based evaluation of a CBT-I digital therapeutic. *Presented at CIST 2025; in preparation for journal submission.*

**Essay 3.** AI Underwriting in Health Insurance, from Model to Market. Develops an AI underwriting model and examines how insurers should allocate decisions among rules, human judgment, and AI, in collaboration with KB Life Insurance, a major South Korean life insurer. *Field experiment in preparation on how the model's risk information shapes underwriting decisions and individuals' responses.*

### Publications

<div class="paper" markdown="1">

Kim, J., **Yoon, S.**, Chung, S., & Oh, W. (2025). Working Daily, Paid Monthly? Effects of On-Demand Wage Access on the Financial Engagement of Low-Wage Workers. *Information Systems Research* 37(3):1463–1484.
{: .paper__cite}

*My role:* responsible for the causal machine learning analyses (double/debiased machine learning, causal forest); conducted the semistructured user interviews.
{: .paper__role}

<p class="links"><a class="chip" href="https://doi.org/10.1287/isre.2023.0673">DOI</a></p>

<details markdown="1">
<summary>Abstract</summary>

Shows that on-demand wage access (OWA) increases low-wage workers' saving frequency, financial-dashboard monitoring, and explicit goal-setting by giving them more autonomy over when they use their income. Combining transaction data from about 4,000 workers with an online experiment, a 58-respondent survey, and 20 interviews, the mixed-methods design traces these gains to a self-empowerment mechanism: workers shift from reactive to proactive financial management, using OWA as scaffolding for disciplined saving behavior.

</details>

</div>

### Working Papers

<div class="paper" markdown="1">

Kim, K., **Yoon, S.**, Kwon, H.E., & Oh, W. Rational App Curation: A Portfolio-Theoretic View of Mobile App Adoption and Churn. *Preparing submission to Information Systems Research.*
{: .paper__cite}

*My role:* co-developing the framework that connects the multiple discrete-continuous extreme value (MDCEV) model to a deep learning forecasting component, feeding MDCEV-estimated parameters into the network as inputs.
{: .paper__role}

<details markdown="1">
<summary>Abstract</summary>

Models app adoption and churn as portfolio decisions: users weigh each app's utility against its risk of usage satiation, with multi-homing acting as diversification across their "app portfolio." Structural estimates of app-level utility and satiation risk are used to build individualized efficient frontiers, and folding these portfolio features into machine-learning predictions improves adoption and churn accuracy by up to 8.6 and 9.1 percentage points, respectively, over behavioral, demographic, affinity-driven, and network-based benchmarks.

</details>

</div>

<div class="paper" markdown="1">

Kim, J., **Yoon, S.**, Ghose, A., & Oh, W. Beyond Efficiency: The Impact of Self-Order Kiosk Adoption on Demand Variety. *Preparing submission to Production and Operations Management.*
{: .paper__cite}

*My role:* built the store-level structural model of kiosk adoption and conducted the interviews that strengthen the qualitative case for the mechanism.
{: .paper__role}

<details markdown="1">
<summary>Abstract</summary>

Using a staggered difference-in-differences design on 17 months of transaction data from a major Korean coffee franchise, shows that self-order kiosk adoption immediately widens demand variety, both across menu items and in customization intensity, as kiosks lower the social friction of complex orders and surface long-tail items. The expansion persists longer in lower-income districts and fades faster in affluent ones, producing an asymmetric split in which headquarters keep the revenue gains while franchisees absorb the added operational complexity.

</details>

</div>

<div class="paper" markdown="1">

Kim, K., **Yoon, S.**, Park, J., Lee, G., & Lee, D. What Algorithms Leave Behind: How Automatic Matching Reshapes Worker Capability in Ride-Hailing Platforms. *Accepted, ICIS 2026. Targeted for Information Systems Research or Management Science.*
{: .paper__cite}

*My role:* developing a structural model complementing the main empirical analysis.
{: .paper__role}

<details markdown="1">
<summary>Abstract</summary>

Tracking drivers on a South Korean ride-hailing platform as they move into and out of an automatic-matching system that limits their discretion over which rides to accept, finds that automatic matching reduces cruising time but also erodes drivers' alignment with recurring and unusual demand patterns. After drivers regain discretion, alignment with recurring demand largely recovers while alignment with unusual demand only partially does, suggesting algorithmic delegation reshapes different dimensions of worker skill unevenly depending on how much practice, feedback, and relearning the system leaves room for.

</details>

</div>

<div class="paper" markdown="1">

Park, J., **Yoon, S.**, Shin, D., & Cho, D. When Does a Pickup Become a Commitment? Dynamic Decision Boundaries and Temporal Graph Learning in Cashierless Retail Stores. *Preparing submission to Manufacturing & Service Operations Management.*
{: .paper__cite}

*My role:* independently developed the deep learning model for the research question and context (the Dynamic Heterogeneous Temporal Commitment Network).
{: .paper__role}

<details markdown="1">
<summary>Abstract</summary>

Argues that cashierless stores relocate the observable purchase decision from checkout to the seconds right after a shopper picks up an item, the *physical commitment boundary* between a shelf return and a carry-forward purchase. Linking shelf-event logs, LiDAR trajectories, and payment records from a cashierless store, the proposed network combines relation-specific graph attention over nearby shoppers with a causal temporal convolutional network over the focal shopper's own trajectory to forecast, in real time and without lookahead, whether a picked-up item will be returned or bought.

</details>

</div>

<div class="paper" markdown="1">

Park, D., Yu, W., & **Yoon, S.** (authors in alphabetical order). Designing a Trustworthy AI Artifact for Emotion Measurement in Consumer Reviews: An Appraisal Theory-Driven Concept-Bottleneck Approach. *Preparing submission to Journal of Marketing.*
{: .paper__cite}

*My role:* selected the theoretical framework (the OCC appraisal model) and developed a new prediction model, OCC-ToneNet.
{: .paper__role}

<details markdown="1">
<summary>Abstract</summary>

Proposes OCC-ToneNet, a concept-bottleneck model that grounds emotion measurement in consumer reviews in Ortony-Clore-Collins appraisal theory, so that every prediction is composed from interpretable, theory-specified concepts rather than an opaque neural mapping. Against fine-tuned language-model baselines on Amazon reviews, the theory-constrained model gives up only about 0.01 in correlation with reference scores while guaranteeing directional consistency by construction, and scaling its encoder closes even that small gap.

</details>

</div>

<div class="paper" markdown="1">

Bhaek, J., Choi, K., & **Yoon, S.** (authors in alphabetical order). Structure-aware Human–AI Reciprocal Estimation: Recovering Preference Structure from Generative AI under Human-Data Scarcity. *Under review at Information Systems Research.*
{: .paper__cite}

*My role:* equal contribution; co-developed the estimator that pools response distributions from multiple generative AI services with scarce human-response data.
{: .paper__role}

<details markdown="1">
<summary>Abstract</summary>

Develops Structure-aware Human–AI Reciprocal Estimation (SHARE), which combines limited human data with LLM-generated choices to estimate preference structure. SHARE allows LLM-specific response scales and attribute-level differences, then uses human response information to calibrate the overall coefficient magnitude. Across two conjoint-choice settings, SHARE most consistently improves recovery of preference structure when human data are scarce, and a multi-model extension that jointly uses several LLMs reduces dependence on selecting a favorable model in advance.

</details>

</div>

### Conference Presentations

Kim, K., **Yoon, S.**, Park, J., Lee, G., & Lee, D. What Algorithms Leave Behind: How Automatic Matching Reshapes Worker Capability in Ride-Hailing Platforms. **ICIS 2026** (forthcoming).

**Yoon, S.**, Oh, J., & Oh, W. Screening Mental Health with Smartphones: Understanding Real-World Noise in Smartphone-Generated Physiological Data. **CIST 2026** and **ICIS 2026** (forthcoming).

Kim, K., Kang, H., Lee, D., Lee, G., Park, J., & **Yoon, S.** Unintended Consequences of Algorithmic Management: Evidence from Automatic Matching Systems in Ride-Hailing Platforms. **PACIS 2026.**

Kang, H., Kim, K., **Yoon, S.**, Lee, G., & Lee, D. Non-Punitive Governance in Algorithmic Markets: The Role of Tag-Based Feedback in Ride-Hailing. **WISE 2025.**

**Yoon, S.**, Ko, S.G., & Oh, W. Engaging for Better Sleep: User Interaction and Behavioral Change in a Mobile App-Based Digital Therapeutic for Insomnia. **CIST 2025.**

Kim, J., & **Yoon, S.** Could Self-Order Kiosks Drive Unequal Demand Trends? An Analysis of How Kiosks Influence Stores and Demand Variety. **WISE 2024.**

Heo, W., **Yoon, S.**, Han, S.P., & Oh, W. When the Human-Algorithm Voice Connection Fails: Effects of Attribution Responses on User Engagement with AI-Enabled Smart Speakers. **CIST 2023.**

Kim, J., **Yoon, S.**, & Chung, S. Working Daily, Paid Monthly? Effects of On-Demand Earned Wage Access on the Financial Well-Being of Low-Wage Workers. **CIST 2023.**

### Industry and Data Partnerships

**KB Life Insurance**, a South Korean life insurer under KB Financial Group (Apr. 2026 to present). Development of an AI underwriting model and a planned field experiment on AI-generated health risk information.

**Kakao Mobility**, Korea's dominant ride-hailing platform (Nov. 2023 to Mar. 2024). Data value assessment for platform-generated matching data, drawing on approximately 48 million driver-passenger match attempts. Informs the *What Algorithms Leave Behind* working paper.

**Shinhan Card**, one of Korea's largest credit card companies (Aug. 2023 to Dec. 2024). AI-based call center service improvement.

## Teaching

### Instructor

**Big Data Programming I**, Department of Big Data Applications, Kyung Hee University. Mar. 2026 to Jul. 2026.  
Introductory Python programming course; sole instructor, 87 students. Teaching evaluation: 94.67 / 100 (department average 94.49).

### Corporate and Executive Education

**Vibe Coding (AI-Assisted Software Development) and Deep Learning.** Kia Corporation, an automaker under Hyundai Motor Group. 2026.

**Machine Learning and Deep Learning for the Insurance Industry.** Heungkuk Life Insurance. 2025.

**Causal Machine Learning.** TMAP Mobility, Korea's leading navigation and mobility platform. 2023.

**Machine Learning and Deep Learning.** Samsung Electro-Mechanics, an electronic-components affiliate of Samsung Group. 2022.

**Machine Learning.** Hyundai Motor Group. 2021.

**Machine Learning.** LG Group. 2021.

### Guest Lectures

**Large language models.** Kyung Hee University, Fall 2025.

**Agentic AI.** Kyung Hee University, Spring 2025.

**Difference-in-differences methodology.** Digital and Platform Business (MBA), KAIST College of Business, Fall 2023.

**Korea's economic development.** Korean Society and Culture, an International MBA course for students from South America, Africa, the Middle East, and Southeast Asia, KAIST College of Business, Fall 2022.

### Teaching Assistant

**AI-Driven Business Evolution** (MBA), KAIST College of Business. Mar. 2026 to Jul. 2026.  
Co-designed the syllabus and evaluation rubrics for a course in which students build agentic AI and LLM-based MVP web or mobile services. Conducted business-viability review and feedback.

**Cloud Computing and Unstructured Data Analytics**, KAIST College of Business. Mar. 2023 to Jul. 2023.  
Supported student projects on AWS-based collection and analysis of unstructured text data.

### Curriculum Development

**KCB Math Camp and KCB AI Camp**, KAIST College of Business. Feb. 2024.  
Designed and taught both camps (curriculum, syllabus, and instruction) for incoming master's and doctoral students.

**Deep Learning for Computer Vision**, Modulabs online learning platform. 2023.  
Designed and recorded a self-paced online course for non-specialists with basic Python experience (11 lectures, 13 h 20 min). [Course page](https://class.modulabs.co.kr/classes/74).

## Background

### Education

**Ph.D. in Management Engineering (Information Systems Track)**  
KAIST College of Business, Seoul, Korea. Mar. 2022 to expected Aug. 2027.  
Advisor: Professor Wonseok Oh. Dissertation proposal defended May 2026; final defense planned for April 2027.

**M.S. in Business Administration (Marketing)**  
Korea University Business School, Seoul, Korea. Mar. 2017 to Aug. 2019.  
Thesis: "Exploring Mechanism of Marriage Decision: Hierarchical Bayesian Approach."  
GPA: 4.20 / 4.50 (96.6 / 100).  
Awards: Best Thesis Proposal Award; Best English Thesis Award.

**B.B.A. in Business Administration**  
Korea University, Seoul, Korea. Mar. 2009 to Feb. 2017.  
GPA: 4.34 / 4.50 (98.4 / 100).  
Exchange student, University of Illinois, 2014.

### Grants and Awards

**Selected Participant**, INFORMS Information Systems Society (ISS) Doctoral Consortium. 2026.

**Doctoral Student Research Encouragement Grant**, National Research Foundation of Korea. 2024 to 2026. KRW 20,000,000 over two years.

**Best Thesis Proposal Award**, Korea University Business School Graduate School. 2019.

**Best English Thesis Award**, Korea University Business School Graduate School. 2019.

**Army Commendation Medal (ARCOM)**, United States Army, for meritorious service as a Sergeant in the USFK Public Affairs Office. Awarded January 21, 2012.

### Service

**Ad hoc reviewer, conferences.** ICIS (2022, 2023, 2024, 2026); PACIS (2023, 2024); CIST (2026).

**Ad hoc reviewer, journals.** Asia Pacific Journal of Information Systems (4 manuscripts); Decision Sciences Journal (1 manuscript).

### Doctoral Coursework

Panel Data Econometrics · Applied Econometrics · Microeconomic Analysis · Industrial Organization · Behavioral Economics: Theory and Applications · Quantitative Models for Marketing Decisions · Multivariate Statistical Analysis · Machine Learning for AI · Bayesian Machine Learning

### Earlier Professional Experience

**Research Intern**, Oliver Wyman, a global management consulting firm. 2016.  
Analyzed the overseas performance of a Korean property insurer and researched international pricing practices.

**Sales Team Intern**, Tree Planet, a Korean social venture in reforestation. 2015.  
Corporate and individual sales, new business development, and quantitative assessment of social and economic impact.

**Founding Member**, Taling, a skill-sharing startup that has since become one of Korea's major online education platforms. 2015.

**Founding Member**, BeKind, a donation platform that has since become Shoot for Love, one of Korea's leading football content channels. 2012.

### Military Service

**Republic of Korea Army**, assigned to United States Forces Korea (USFK Public Affairs Office). Jun. 2010 to Feb. 2012.  
Completed mandatory military service in a combined United States and Korean command, working in English daily.

### Technical Skills

**Programming and statistical software.** Python, R, Stata.  
**Languages.** Korean (native), English (fluent).

---

Reach me at [seokchaeyoon@kaist.ac.kr](mailto:seokchaeyoon@kaist.ac.kr).
