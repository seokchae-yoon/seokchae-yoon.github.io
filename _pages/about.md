---
permalink: /
title: "Seokchae Yoon"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a Ph.D. candidate in Management Engineering (Information Systems) at the KAIST College of Business, advised by Professor Wonseok Oh. I expect to complete my degree in 2027, and I am on the job market this year.

My research asks when AI-generated information can be trusted, and what that trust is worth to the individuals, professionals, and firms that act on it. My dissertation pursues this question in healthcare, from smartphone-based mental health screening to AI underwriting in insurance markets. I carry the same lens into digital platforms and retail, building the model each setting requires.

**Research areas.** Healthcare IT, algorithmic decision-making, platform economics.  
**Methods.** Deep learning, econometrics and causal inference, Bayesian statistics and machine learning.

## Job Market Paper

**Screening Mental Health with Smartphones: Understanding Real-World Noise in Smartphone-Generated Physiological Data**  
Yoon, S., Oh, J., & Oh, W.  
*Under review at MIS Quarterly.* To be presented at CIST 2026.

<details markdown="1">
<summary>Abstract</summary>

Develops a biodynamics-guided deep learning framework for smartphone-based depression screening that quantifies real-world measurement noise through deep-ensemble uncertainty estimation, addressing the reliability problem that limits consumer-grade digital biomarkers.

</details>

## Research

### Dissertation

**When AI Enters the Healthcare Information Environment: Sensing, Treatment, and Markets**  
Committee Chair: Professor Wonseok Oh. Proposal defended May 2026.

The dissertation examines what happens when AI relaxes long-standing information constraints in healthcare, across three essays spanning physiological screening, behavioral treatment delivery, and risk-based market design. It argues that the value of AI-generated health information is not fixed, but depends on the reliability of the information the AI produces, the mechanism through which it reaches individuals, and the market structure it enters.

**Essay 1 (Job Market Paper).** Screening Mental Health with Smartphones: Understanding Real-World Noise in Smartphone-Generated Physiological Data. *Under review at MIS Quarterly.*

**Essay 2.** Engaging for Better Sleep: User Interaction and Behavioral Change in a Mobile App-Based Digital Therapeutic for Insomnia. An RCT-based evaluation of a CBT-I digital therapeutic. *Presented at CIST 2025; in preparation for journal submission.*

**Essay 3.** AI Underwriting in Health Insurance: Model Development and Market Consequences. Develops an AI underwriting model and tests a human-AI decision delegation design (Always Rule / Selective AI / Always AI) through a pre-registered field experiment, in collaboration with KB Life. *Under review, WISE 2026; pre-registered field experiment forthcoming.*

### Publications

Kim, J., **Yoon, S.**, Chung, S., & Oh, W. (2025). Working Daily, Paid Monthly? Effects of On-Demand Wage Access on the Financial Engagement of Low-Wage Workers. *Information Systems Research.*  
*My role:* second author. Led the causal-inference and mixed-methods analysis — matrix completion, causal forest, and other causal ML methods — together with the online experiment, survey, and interview components.

<details markdown="1">
<summary>Abstract</summary>

Shows that on-demand wage access (OWA) increases low-wage workers' saving frequency, financial-dashboard monitoring, and explicit goal-setting by giving them more autonomy over when they use their income. Combining transaction data from about 4,000 workers with an online experiment, a 58-respondent survey, and 20 interviews, the mixed-methods design traces these gains to a self-empowerment mechanism: workers shift from reactive to proactive financial management, using OWA as scaffolding for disciplined saving behavior.

</details>

### Working Papers

Kim, K., **Yoon, S.**, Kwon, H.E., & Oh, W. Rational App Curation: A Portfolio-Theoretic View of Mobile App Adoption and Churn. *Preparing submission to Information Systems Research.*  
*My role:* built the structural model, extending the MDCEV framework to the mobile-app-usage setting.

<details markdown="1">
<summary>Abstract</summary>

Models app adoption and churn as portfolio decisions: users weigh each app's utility against its risk of usage satiation, with multi-homing acting as diversification across their "app portfolio." Structural estimates of app-level utility and satiation risk are used to build individualized efficient frontiers, and folding these portfolio features into machine-learning predictions improves adoption and churn accuracy by up to 8.6 and 9.1 percentage points, respectively, over behavioral, demographic, affinity-driven, and network-based benchmarks.

</details>

Kim, J., **Yoon, S.**, Ghose, A., & Oh, W. Beyond Efficiency: The Impact of Self-Order Kiosk Adoption on Demand Variety. *Preparing submission to Production and Operations Management.*  
*My role:* built the store-level structural model of kiosk adoption and conducted the interviews that strengthen the qualitative case for the mechanism.

<details markdown="1">
<summary>Abstract</summary>

Using a staggered difference-in-differences design on 17 months of transaction data from a major Korean coffee franchise, shows that self-order kiosk adoption immediately widens demand variety, both across menu items and in customization intensity, as kiosks lower the social friction of complex orders and surface long-tail items. The expansion persists longer in lower-income districts and fades faster in affluent ones, producing an asymmetric split in which headquarters keep the revenue gains while franchisees absorb the added operational complexity.

</details>

Kim, K., **Yoon, S.**, Park, J., Lee, G., & Lee, D. What Algorithms Leave Behind: How Automatic Matching Reshapes Worker Capability in Ride-Hailing Platforms. *Conditionally accepted, ICIS 2026; preparing submission to Management Science.*  
*My role:* led the empirical analysis and the interview-based qualitative work.

<details markdown="1">
<summary>Abstract</summary>

Tracking drivers on a South Korean ride-hailing platform as they move into and out of an automatic-matching system that limits their discretion over which rides to accept, finds that automatic matching reduces cruising time but also erodes drivers' alignment with recurring and unusual demand patterns. After drivers regain discretion, alignment with recurring demand largely recovers while alignment with unusual demand only partially does, suggesting algorithmic delegation reshapes different dimensions of worker skill unevenly depending on how much practice, feedback, and relearning the system leaves room for.

</details>

Park, J., **Yoon, S.**, Shin, D., & Cho, D. When Does a Pickup Become a Commitment? Dynamic Decision Boundaries and Temporal Graph Learning in Cashierless Retail Stores. *Under review, WITS 2026; preparing submission to Manufacturing & Service Operations Management.*  
*My role:* designed and built the proposed model, the Dynamic Heterogeneous Temporal Commitment Network.

<details markdown="1">
<summary>Abstract</summary>

Argues that cashierless stores relocate the observable purchase decision from checkout to the seconds right after a shopper picks up an item, the *physical commitment boundary* between a shelf return and a carry-forward purchase. Linking shelf-event logs, LiDAR trajectories, and payment records from a cashierless store, the proposed network combines relation-specific graph attention over nearby shoppers with a causal temporal convolutional network over the focal shopper's own trajectory to forecast, in real time and without lookahead, whether a picked-up item will be returned or bought.

</details>

Park, D., Yu, W., & **Yoon, S.** (authors in alphabetical order). Designing a Trustworthy AI Artifact for Emotion Measurement in Consumer Reviews: An Appraisal Theory-Driven Concept-Bottleneck Approach. *Under review, WITS 2026; preparing submission to Journal of Marketing.*  
*My role:* designed and built the proposed model, OCC-ToneNet.

<details markdown="1">
<summary>Abstract</summary>

Proposes OCC-ToneNet, a concept-bottleneck model that grounds emotion measurement in consumer reviews in Ortony-Clore-Collins appraisal theory, so that every prediction is composed from interpretable, theory-specified concepts rather than an opaque neural mapping. Against fine-tuned language-model baselines on Amazon reviews, the theory-constrained model gives up only about 0.01 in correlation with reference scores while guaranteeing directional consistency by construction, and scaling its encoder closes even that small gap.

</details>

Bhak, J., Choi, K., & **Yoon, S.** (authors in alphabetical order). Leveraging Preference Structure from LLM-Generated Choices: A Scale-Adjusted Pooling Approach. *Under review, WITS 2026; preparing submission to Information Systems Research.*  
*My role:* co-developed the proposed estimator with the other authors, using LLM-generated data to augment it.

<details markdown="1">
<summary>Abstract</summary>

Proposes Scale-Adjusted Structural Pooling (SASP), an estimator that combines a large sample of LLM-generated choices with a small human sample by assuming both share a preference direction while keeping source-specific utility scales — letting the LLM data pin down the direction of the human coefficient vector while the human data calibrates its scale. Across two conjoint datasets, SASP improves coefficient recovery over benchmark estimators, especially when the LLM's preference structure is compatible with the human target and the human sample is small.

</details>

### Conference Presentations

Kim, K., Kang, H., Lee, D., Lee, G., Park, J., & **Yoon, S.** Unintended Consequences of Algorithmic Management: Evidence from Automatic Matching Systems in Ride-Hailing Platforms. **PACIS 2026.**

Kang, H., Kim, K., **Yoon, S.**, Lee, G., & Lee, D. Non-Punitive Governance in Algorithmic Markets: The Role of Tag-Based Feedback in Ride-Hailing. **WISE 2025.**

**Yoon, S.**, Ko, S.G., & Oh, W. Engaging for Better Sleep: User Interaction and Behavioral Change in a Mobile App-Based Digital Therapeutic for Insomnia. **CIST 2025.**

Kim, J., & **Yoon, S.** Could Self-Order Kiosks Drive Unequal Demand Trends? An Analysis of How Kiosks Influence Stores and Demand Variety. **WISE 2024.**

Heo, W., **Yoon, S.**, Han, S.P., & Oh, W. When the Human-Algorithm Voice Connection Fails: Effects of Attribution Responses on User Engagement with AI-Enabled Smart Speakers. **CIST 2023.**

Kim, J., **Yoon, S.**, & Chung, S. Working Daily, Paid Monthly? Effects of On-Demand Earned Wage Access on the Financial Well-Being of Low-Wage Workers. **CIST 2023.**

### Industry and Data Partnerships

**KB Life Insurance**, a life insurer under KB Financial Group (2026 to present). Development of an AI underwriting model and a pre-registered field experiment on human-AI decision delegation.

**Kakao Mobility**, Korea's dominant ride-hailing platform (2024). Data value assessment for platform-generated matching data, drawing on approximately 48 million driver-passenger match attempts. Informs the *What Algorithms Leave Behind* working paper.

**Shinhan Card**, one of Korea's largest credit card companies (2023). AI-based call center service improvement.

## Teaching

### Instructor

**Big Data Programming I**, Department of Big Data Applications, Kyung Hee University. Spring 2026.  
Introductory Python programming course. Teaching evaluation: 94.67 / 100 (department average 94.49).

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

**AI-Driven Business Evolution**, KAIST College of Business. Spring 2026.  
Co-designed the syllabus and evaluation rubrics for a course in which students build agentic AI and LLM-based MVP web or mobile services. Conducted business-viability review and feedback.

**Cloud Computing and Unstructured Data Analytics**, KAIST College of Business. Spring 2023.  
Supported student projects on AWS-based collection and analysis of unstructured text data.

### Curriculum Development

**Math Camp and AI Camp**, KAIST College of Business. 2024.  
Designed and delivered both curricula for incoming graduate students.

## Background

### Education

**Ph.D. in Management Engineering (Information Systems Track)**  
KAIST College of Business, Seoul, Korea. Mar. 2022 to expected 2027.  
Advisor: Professor Wonseok Oh. Dissertation proposal defended May 2026.

**M.A. in Business Administration (Marketing)**  
Korea University Business School, Seoul, Korea. Mar. 2017 to Aug. 2019.  
Thesis: "Exploring Mechanism of Marriage Decision: Hierarchical Bayesian Approach."  
Awards: Best Thesis Proposal Award; Best English Thesis Award.

**B.A. in Business Administration**  
Korea University, Seoul, Korea. Mar. 2009 to Aug. 2016.  
Exchange student, University of Illinois, 2014.

### Grants and Awards

**Doctoral Student Research Encouragement Grant**, National Research Foundation of Korea. 2024 to 2026. KRW 20,000,000 over two years.

**Best Thesis Proposal Award**, Korea University Business School Graduate School. 2019.

**Best English Thesis Award**, Korea University Business School Graduate School. 2019.

**Army Commendation Medal (ARCOM)**, United States Army, for meritorious service. 2012.

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

**Republic of Korea Army**, assigned to United States Forces Korea. 2010 to 2012.  
Completed mandatory military service in a combined United States and Korean command, working in English daily.

### Technical Skills

**Programming and statistical software.** Python, R, Stata.  
**Languages.** Korean (native), English (fluent).

---

Reach me at [seokchaeyoon@kaist.ac.kr](mailto:seokchaeyoon@kaist.ac.kr).
