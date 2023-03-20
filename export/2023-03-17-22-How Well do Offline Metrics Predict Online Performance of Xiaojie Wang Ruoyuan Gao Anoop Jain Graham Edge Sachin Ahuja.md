## Paper:1




1. Title: How Well do Offline Metrics Predict Online Performance of Product Ranking Models?

2. Authors: Xiaojie Wang, Ruoyuan Gao, Anoop Jain, Graham Edge, Sachin Ahuja

3. Affiliation: Xiaojie Wang - Amazon.com, Palo Alto, CA, USA

4. Keywords: Evaluation metrics, online evaluation, offline evaluation

5. Url: https://dl.acm.org/doi/10.1145/3077136.3080797
Github: None

6. Summary:

- (1): The paper addresses the challenge of using offline metrics to effectively select ranking models for online experiments by studying how well offline metrics predict the performance of product search ranking models in online evaluations.
 
- (2): Past methods include online evaluation through A/B testing and interleaving methods; however, they have limitations such as testing only a limited number of models and the risk of deteriorating user search experience. The approach in this paper is well motivated because offline evaluation can test a larger number of models and using offline metrics with high agreement with online metrics can select models that have better performance in online evaluations.

- (3): The research methodology involves collecting gold data in the form of preferences over ranker pairs under a business metric in an e-commerce search engine. The gold data is used to evaluate offline metrics in terms of their directional agreement with the business metric, their discriminative power through paired sample t-test and rank correlations among offline metrics. The study involves 36 offline metrics and extensive online and offline experiments on Amazon search ranking data.

- (4): The methods in the paper achieve high agreement between offline and online metrics, with 97% agreement on which ranking model is better. The offline metrics are highly discriminative on large-scale search ranking data, especially NDCG which has a discriminative power over 99%.

7. Strengths and Weaknesses:

Strengths:
- Originality: The paper studies how well offline metrics predict online performance for product search ranking models, which has not been studied extensively before.
- Quality: The paper provides a thorough evaluation of 36 offline metrics and their agreement and discriminative power with online metrics.
- Clarity: The paper is well-written and organized, making it easy to understand the research methodology and results.

Weaknesses:
- Significance: While the paper has practical implications for selecting ranking models in e-commerce search engines, the impact on other domains may be limited.
- Scope: The paper focuses only on product search ranking models, which may limit its generalizability to other ranking applications.
- Assumptions: The paper assumes that the business metric used in the gold data accurately reflects user preferences, which may not always be the case.





8. Conclusion:

- (1): This study is significant because it addresses the challenge of using offline metrics to select ranking models for online experiments. The paper provides a thorough evaluation of offline metrics and their agreement and discriminative power with online metrics. The findings can be applied in e-commerce search engines to effectively select ranking models for better user search experience.

- (2): Innovation point: The paper studies how well offline metrics predict online performance for product search ranking models, which has not been extensively studied before. Performance: The research achieves a high degree of agreement and discriminative power between offline and online metrics, with NDCG having over 99% discriminative power. Workload: The paper involves collecting gold data and evaluating 36 offline metrics, which may require significant resources for replication.




