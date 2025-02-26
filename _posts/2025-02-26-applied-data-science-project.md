---
layout: post
author: Gwen
title: "Applied Data Science Project Documentation"
categories: ITD214
---
## Project Background

Analyse global news, industry discussions, government policies, and customer feedback from Jan 2024
till-date, to help Tech giant (Apple) identify risks and/or opportunities and plan for its next iPhone rollout

![image](https://github.com/user-attachments/assets/5ff41fd4-0c45-450c-836f-78826a1e7af5)

## Work Accomplished

Business Objective #2: Detect trends in industry discussions and government policies using keyword and topic analysis from public reports

Success Criteria:
Factors and Services that will be counted on to:
1. Drive growth.
2. Increase Revenue per user.
3. Lock in users to the Ecosystem.

### Data Understanding

* Data Source

_Gartner Press Releases_: Focus on reports related to Apple’s industry and relevant tech trends.
_Google News, ChannelNewsAsia and MacDailyNews_: News articles and reports covering Apple, government policies and trends.

![Picture1](https://github.com/user-attachments/assets/cd8824bc-dc6f-4e78-8b99-8653e5313aa1)

![Picture2](https://github.com/user-attachments/assets/5c5c166f-12ce-4c10-b96a-e719bc747dfa)

* Data Breakdown

Data were extracted from Gartner reports, Google News, ChannelNewsAsia, MacDailyNews using Octoparse for the year 2024.

* Gartner report (432 rows for 2024)
  
![Picture3](https://github.com/user-attachments/assets/ca837e78-b5cc-4b7d-93b5-9d6a8846bf00)

  
* Google news, ChannelNewsAsia, MacDailyNews (340 rows)
  
![Picture4](https://github.com/user-attachments/assets/8f6c8dbf-2913-488f-bf9d-83defc58cecd)

![Picture5](https://github.com/user-attachments/assets/088c30fc-06d3-4da4-bcc7-bf3dd01f30fd)



### Data Preprocessing

Data preprocessing includes cleaning of dataset, checking of missing values, imputation/replacement of missing values, lemmatization, removing of stop words, links, punctuations and hashtags. Stop words list are reviewed and then adjusted to show only words that are of significance.

- Handling of Missing Values

![Picture6](https://github.com/user-attachments/assets/d9c46a51-f388-4be1-900f-3c8080b56e9b)


- Removal of Stopwords

![Picture7](https://github.com/user-attachments/assets/13e36da7-17e1-4af4-84f7-6d542de85a18)


- Tokenization and Lemmatization

![Picture8](https://github.com/user-attachments/assets/5d208fca-dc5f-4911-b2e4-c90ebd2af4a5)

  
Top 20 Most Frequent Words in Texts

Gartner's Report

![Picture9](https://github.com/user-attachments/assets/7bc58c47-6601-4e01-83ab-4eadad330f14)



Google News, ChannelNewsAsia, MacDailyNews

![Picture10](https://github.com/user-attachments/assets/7e185b37-059e-4199-ac9e-095de367e281)

Words Clouds

![Picture11](https://github.com/user-attachments/assets/2e19e3d9-bbb7-427d-a631-517f7639ad45)



### Topic Modelling with LDA

* Checking the number of topics, coherence score and perplexity score

![Picture12](https://github.com/user-attachments/assets/d8942a16-ce7f-4fe7-8440-49783a848c38)



![Picture13](https://github.com/user-attachments/assets/f0cba8c3-2549-4bc2-be16-82209f967cf1)


* Visualization of the topic words and clusters
  
![Picture14](https://github.com/user-attachments/assets/bc9d56e2-0ec1-4511-93d5-39e352051a06)

![Picture15](https://github.com/user-attachments/assets/1b1ab7af-366b-4ca0-baf8-b4559b6dc4d5)

![Picture16](https://github.com/user-attachments/assets/5f54b086-60c5-4fa9-a8f6-643adf4b266b)


### Evaluation

* Analysizing the topics words
  
Part 1 - Gartner’s Reports
Topic Words

1. 0.017*"strategy" + 0.013*"ai" + 0.013*"marketing" + 0.011*"cloud" + 0.009*"customer" + 0.007*"infrastructure" + 0.007*"service" + 0.007*"operation" + 0.006*"cybersecurity" + 0.006*"compliance"
2. 0.029*"supply" + 0.028*"chain" + 0.027*"ai" + 0.018*"data" + 0.011*"analytics" + 0.011*"risk" + 0.010*"marketing" + 0.010*"growth" + 0.008*"management" + 0.008*"security"
3. 0.023*"finance" + 0.009*"ai" + 0.009*"risk" + 0.008*"genai" + 0.008*"supply" + 0.006*"customer" + 0.006*"transformation" + 0.005*"data" + 0.005*"digital" + 0.005*"legal"


Part 2 - Google News, ChannelNewsAsia, MacDailyNews
Topic Words

1. 0.021*"eu" + 0.019*"antitrust" + 0.011*"ai" + 0.010*"store" + 0.010*"foxconn" + 0.008*"fine" + 0.008*"profit" + 0.006*"lawsuit" + 0.006*"intelligence" + 0.006*"global"
2. 0.018*"eu" + 0.010*"ai" + 0.010*"store" + 0.008*"huawei" + 0.008*"nvidia" + 0.007*"game" + 0.007*"supplier" + 0.006*"valuable" + 0.006*"fine" + 0.006*"regulator"
3. 0.012*"eu" + 0.011*"chip" + 0.009*"io" + 0.007*"lawsuit" + 0.006*"ai" + 0.006*"nvidia" + 0.006*"sport" + 0.006*"exec" + 0.006*"request" + 0.006*"home"
4. 0.020*"ai" + 0.014*"chip" + 0.012*"foxconn" + 0.009*"eu" + 0.009*"india" + 0.009*"tv" + 0.008*"store" + 0.008*"china" + 0.008*"pay" + 0.006*"apps"
5. 0.020*"ai" + 0.015*"pro" + 0.010*"intelligence" + 0.008*"offer" + 0.007*"eu" + 0.007*"pay" + 0.005*"china" + 0.005*"forecast" + 0.005*"indonesia" + 0.005*"probe"



## Recommendation and Analysis

**Part 1 - Gartner's Reports**

Key Findings
 
AI's Pervasive Impact:
- Gartner’s reports reveal that AI is revolutionising services, infrastructure, supply chains, and marketing, driving efficiency and innovation.

Cybersecurity & Privacy Risks:
- AI amplifies cybersecurity threats (social engineering, malicious chatbots, evolving attacks).
- Excessive personalisation and data collection erode consumer trust.
- Fraud risks rise with AI-driven customer service via third-party assistants.

Balancing Innovation & Security:
- Businesses must balance AI-driven innovation with robust cybersecurity and data privacy measures.
- Focus on ethical AI practices, strong data governance, and proactive risk management.

Market Trends, Challenges and Recommendations:
- Target for Attacks: The iPhone can be a prime target for AI-driven social engineering and phishing.
- Customer Service & AI: Apple AI and third-party assistants reshape iPhone user interactions, raising privacy/security concerns.
- Supply Chain & Semiconductors: AI optimises the iPhone's complex supply chain and relies on advanced semiconductors.
- Data & Marketing: Data drives personalised marketing, but Apple's privacy must continue to focus on addressing  user concerns.
- Security & Compliance: Apple has a high degree of hardware and software control. Apple's on-device AI, Private Cloud Compute, and DMA compliance are critical. 

**Part 2 - Google News, ChannelNewsAsia, MacDailyNews**

Key Findings

iPhone Growth Drivers:
- Innovation is Key: Continuous introduction of cutting-edge features (AI chips, enhanced cameras, new apps) drives growth and competitiveness.
- Supply Chain Optimization: Efficient manufacturing (Foxconn) and strategic expansion (India, Indonesia) are crucial.
- Geopolitical Risks: US political changes (potential tariffs) could disrupt production and necessitate supply chain diversification.

Ecosystem & User Lock-in:
- Seamless Integration: Hardware, software, and services create a cohesive user experience, fostering loyalty.
- Service Bundles & App Store: Recurring revenue and a thriving developer ecosystem reinforce user engagement.

Future Trends, Challenges & Recommendations:

- AI & LLM Competition: Apple Intelligence must compete with leading LLMs (ChatGPT, Gemini), requiring significant AI development.
- Legal & Regulatory Landscape: Antitrust lawsuits and EU regulations (DMA) pose significant challenges.
- Compliance & Adaptation: Apple must adapt its strategies to comply with evolving regulations, facing potential fines and operational restrictions.
- Global Legal Battles: Apple will continue to fight legal battles across multiple jurisdictions.





## AI Ethics

#### Privacy and Web Scraping:

Issue: Web scraping can inadvertently collect personal data or sensitive information if not carefully managed. Even if the scraped data is ostensibly public, aggregating large volumes of it can reveal patterns and insights that individuals did not intend to share.

Ethical Concern: Respecting user privacy is paramount. Scraping data without clear consent or without anonymizing or aggregating it can violate ethical principles.

Mitigation:
- Adhere to website terms of service.
- Implement robust anonymization techniques to remove personally identifiable informatio..
- Only scrape data that is absolutely required for the project.

#### Accuracy and Bias in Topic Modeling:

Issue: Topic modeling relies on algorithms that can be influenced by biases present in the training data. If the scraped data disproportionately represents certain viewpoints or demographics, the resulting topics may be skewed.

Ethical Concern: Biased topic models can lead to inaccurate or misleading insights, potentially reinforcing harmful stereotypes or misrepresenting public opinion.

Mitigation:
- Critically evaluate the sources of scraped data for potential biases.
- Employ techniques to balance the dataset and mitigate the impact of biases.
- Clearly disclose any potential biases in the analysis and interpretation of results.
- Validate the topic models with human review and external data sources.


#### Transparency and Reproducibility:

Issue: The process of web scraping and topic modeling can be complex, involving numerous data transformations and algorithmic choices. Without clear documentation, it can be difficult to understand how the results were obtained or to reproduce them.

Ethical Concern: Lack of transparency undermines trust in the analysis and makes it difficult to hold researchers accountable for their findings.

Mitigation:
- Maintain detailed documentation of all data scraping, preprocessing, and modeling steps.
- Clearly explain the limitations and assumptions of the analysis.


#### Accountability and Potential Misuse:

Issue: The insights generated from the project could be used for various purposes, some of which may have unintended consequences. For example, the analysis could be used to manipulate public opinion or to target specific groups with marketing campaigns.

Ethical Concern: Researchers have a responsibility to consider the potential impact of their work and to take steps to prevent its misuse.

Mitigation:
- Clearly define the intended use of the analysis and avoid promoting harmful applications.
- Consider the potential for misuse and implement safeguards to prevent it.





## Source Codes and Datasets
Model files and dataset. 

[https://github.com/gwen-toh/itd214project](https://github.com/gwen-toh/itd214project)


