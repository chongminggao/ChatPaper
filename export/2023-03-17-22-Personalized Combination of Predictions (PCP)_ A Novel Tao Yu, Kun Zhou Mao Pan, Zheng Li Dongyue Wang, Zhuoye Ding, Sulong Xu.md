## Paper:1




1. Title: Personalized Combination of Predictions (PCP): A Novel
   (个性化预测组合（PCP）：一种新的电子商务推荐多任务学习模型)
                 
                 
2. Authors: Tao Yu, Kun Zhou, Mao Pan, Zheng Li, Dongyue Wang, Zhuoye Ding, Sulong Xu

                 
3. Affiliation: JD.com, Inc. Beijing, China


4. Keywords: Multi-task Learning, Personalized Combination, Recommendation System, E-commerce


5. Url: https://dl.acm.org/doi/10.1145/XXXX/XXXX.XXXX


6. Summary:

- (1): This article is about personalized recommendation in e-commerce and the use of multi-task learning (MTL) models to estimate multiple targets simultaneously. However, MTL models suffer from trade-offs between user intent diversity and competing correlation of different tasks which affects the final predictions. Therefore, this paper introduces a novel Personalized Combination of Predictions (PCP) model to address these issues.
 
- (2): Traditional methods of combining multiple predictions in MTL models rely on static combination weights, which are suboptimal in any scenario. Tuning the combination weights manually or using Bayesian Optimization does not take into account users' different intentions, and can lead to a significant seesaw phenomenon. The proposed PCP model utilizes a special expert network to model user intention and calculate personalized combination weights. An efficiently alternating training technique was applied to update the parameters of the special expert network and the main MTL network separately. The approach is well motivated and addresses a key issue for personalized recommendation systems.

- (3): The proposed PCP model is a multi-task learning (MTL) model that includes a component explicitly modeling combination weights based on a special expert network to model user intention. The proposed model uses an efficient alternating training technique to update both the special expert network and main MTL network, separately.

- (4): The proposed PCP model was evaluated online on a large-scale e-commerce recommendation system and achieved significant promotion in both click-through rate (CTR) and conversion rate (CVR) compared to state-of-the-art MTL models with static combination weights. Extensive offline experiments on both public and production datasets demonstrated that PCP is flexible and effective for a variety of MTL-based models.

7. Strengths and Weaknesses:

Strengths:
- The proposed PCP model addresses key issues with multi-task learning models for personalized recommendation systems.
- The paper introduces a novel approach that utilizes a special expert network to model user intention and calculates personalized combination weights.
- The proposed model achieves significant improvements in both click-through rate and conversion rate compared to state-of-the-art MTL models with static combination weights.

Weaknesses:
- The paper lacks a comparison to other models that have a similar approach in modeling personalized combination weights using expert networks.
- The paper could benefit from a more thorough analysis of the proposed method's performance in scenarios with different data distributions or recommending different types of products.
- Although the paper presents extensive offline experiments, there was no analysis regarding the scalability of the proposed method, and can be an issue in real-world scenarios.
7. Methods: 

- (1): The article proposes a novel Personalized Combination of Predictions (PCP) model for personalized recommendation in e-commerce using multi-task learning (MTL) models to estimate multiple targets simultaneously. The PCP model utilizes a special expert network to model user intention and calculate personalized combination weights, addressing the issue of trade-offs between user intent diversity and competing correlation of different tasks. 

- (2): The PCP model improves upon traditional methods of combining multiple predictions in MTL models that rely on static combination weights, which are suboptimal in any scenario. Instead of tuning the combination weights manually or using Bayesian optimization, the proposed method utilizes a special expert network to model user intention and calculate personalized combination weights, while an efficiently alternating training technique is applied to update the parameters of the expert network and the main MTL network separately. 

- (3): The proposed PCP model is a multi-task learning (MTL) model that includes a component explicitly modeling combination weights based on a special expert network to model user intention. The proposed model uses an efficient alternating training technique to update both the special expert network and main MTL network, separately. Two loss functions are introduced to supervise the learning of the PCP model and MTL model, respectively. The PCP model achieves significant improvements in both click-through rate and conversion rate compared to state-of-the-art MTL models with static combination weights.





8. Conclusion:
- (1): The proposed Personalized Combination of Predictions (PCP) model addresses key issues with multi-task learning models for personalized recommendation systems in e-commerce by introducing a novel approach that utilizes a special expert network to model user intention and calculate personalized combination weights.
- (2): Innovation point: The PCP model introduces a novel approach that utilizes a special expert network to model user intention and calculate personalized combination weights, improving upon traditional methods of combining multiple predictions in MTL models. Performance: The proposed PCP model achieves significant improvements in both click-through rate and conversion rate compared to state-of-the-art MTL models with static combination weights, and is effective for a variety of MTL-based models. Workload: The paper presents an efficient and effective training strategy by introducing alternating training technique and gradient stop mechanism for updating the parameters of the special expert network and the main MTL network separately. However, the paper lacks a comparison to other models with similar approaches and could benefit from a more thorough analysis of performance in scenarios with different data distributions or recommending different types of products.




