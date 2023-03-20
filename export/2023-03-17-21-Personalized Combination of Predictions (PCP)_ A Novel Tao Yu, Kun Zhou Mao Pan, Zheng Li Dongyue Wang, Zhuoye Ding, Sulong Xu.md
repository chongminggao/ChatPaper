## Paper:1




1. Title: Personalized Combination of Predictions (PCP): A Novel (个性化预测融合：一种新型的多任务学习模型用于电商推荐系统)

2. Authors: Tao Yu, Kun Zhou, Mao Pan, Zheng Li, Dongyue Wang, Zhuoye Ding, Sulong Xu

3. Affiliation: JD.com, Inc. (Beijing, China)

4. Keywords: Multi-task Learning, Personalized Combination, Recommendation System, E-commerce

5. Urls: Paper: https://dl.acm.org/doi/10.1145/XXXXX.Github: None.

6. Summary:

- (1): The paper proposes a new multi-task learning (MTL) model that explicitly models personalized combination weights to improve the accuracy of predictions in real-world recommendation scenarios.

- (2): Traditional MTL models suffer from negative transfer and competing correlations of different tasks. Previous efforts to optimize separation and joining of experts and loss weighting overlook the importance of prediction combination. Other works that utilized hyper-parameter tuning methods use suboptimal static weights for all users in any scenario. The proposed PCP model models user intention and calculates personalized combination weights, and uses an efficient alternating training technique to update the MTL parameters separately from the combination weight component.

- (3): The PCP model utilizes a special expert network to model user intention and calculate personalized combination weights. It also applies an efficient alternating training technique to update parameters of the special expert network and the main MTL network, separately.

- (4): The PCP model achieved significant promotion in click-through rate (CTR) and conversion rate (CVR) compared to state-of-the-art MTL models with static combination weights. Extensive offline experiments on both public and production datasets demonstrate that PCP is flexible and effective to be applied to a variety of MTL-based models.
7. Methods:

- (1): The proposed Personalized Combination of Predictions (PCP) model is a multi-task learning (MTL) model that explicitly models personalized combination weights to improve prediction accuracy in real-world recommendation scenarios. 

- (2): The PCP model utilizes a special expert network called the Personalized Combination Expert (PCE) to model user intention and calculate personalized combination weights. The PCE is composed of multilayer perceptrons with ReLU activations and a softmax layer. It shares the bottom inputs with the MTL model, including item embedding, user interests embedding, and other context features. 

- (3): The PCE learns user intention patterns from user history behaviors, such as a user's repeated browsing of a product indicating strong willingness to purchase. The ranking system then assigns more combination weight to the purchase task for that candidate item. 

- (4): Two loss functions supervise the learning of the PCP model. The first loss function, 𝐿𝑀𝑇𝐿, is for the MTL model and is calculated based on prediction and ground truth label. The hyperparameter 𝛼𝑘 balances empirical loss between multiple tasks. The second loss function, 𝐿𝑃𝐶𝐸, is for the PCE and depends on the outputs of the main network. It is set up individually and is calculated based on prediction and ground truth label, and the hyperparameter 𝛽𝑘 balances the loss of individual tasks. 

- (5): An efficient alternating training technique is applied to update parameters of the PCE and the main MTL network separately. 

- (6): The PCP model achieved significant improvement in click-through rate (CTR) and conversion rate (CVR) compared to state-of-the-art MTL models with static combination weights. Extensive offline experiments were conducted on both public and production datasets, demonstrating that PCP is flexible and effective for use in a variety of MTL-based models.





8. Conclusion: 

- (1): The proposed Personalized Combination of Predictions (PCP) model is significant for real-world recommendation scenarios as it improves prediction accuracy by explicitly modeling personalized combination weights through user intention.

- (2): Innovation point: The PCP model's innovation lies in its utilization of a special expert network, the Personalized Combination Expert, to model user intention and calculate personalized combination weights, as well as an efficient alternating training technique to update parameters of the expert network and the main MTL network separately. 
Performance: Extensive offline experiments demonstrate that the PCP model significantly improves click-through rate (CTR) and conversion rate (CVR) compared to state-of-the-art MTL models with static combination weights. The results indicate that the personalized combination weights method alleviates the negative effects of negative transfer and competing correlations of different tasks seen in traditional MTL models. 
Workload: The workload of the proposed PCP model is not specifically mentioned in the article, though the efficient alternating training technique utilized suggests a relatively streamlined approach.




