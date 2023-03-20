## Paper:1




1. Title: Personalized Combination of Predictions (PCP): A Novel (个性化预测组合：一种新的多任务学习模型用于电商推荐)
2. Authors: Tao Yu, Kun Zhou, Mao Pan, Zheng Li, Dongyue Wang, Zhuoye Ding, Sulong Xu
3. Affiliation: JD.com, Inc. (北京京东百货电子商务有限公司)
4. Keywords: Multi-task Learning, Personalized Combination, Recommendation System, E-commerce
5. Urls: Paper: https://dl.acm.org/doi/10.1145/XXXXX.XXXXXX, Github: None
6. Summary:

- (1): The research background of this paper is personalized recommendation in e-commerce and the limitations of multi-task learning models for combining multiple targets.
- (2): Past methods have focused on separating and joining experts and the loss weighting strategy to improve learning efficiency and effectiveness. However, in industrial recommendation applications, improving the precision of each task is insufficient without appropriate combination weights. Traditional methods for obtaining static combination weights overlook differences in users' intentions. The proposed approach is motivated by the need for a model that explicitly models personalized combination weights to improve final results.
- (3): The research methodology proposed in this paper is a novel personalized combination of predictions (PCP) multi-task learning model with a component that models combination weights based on user intention. An alternating training technique effectively updates parameters of the expert network and the main MTL network separately.
- (4): The PCP model achieves significant improvement both in click-through rate (CTR) and conversion rate (CVR) compared to state-of-the-art multi-task learning models with static combination weights. Online evaluation on a large-scale e-commerce recommendation system verifies the effectiveness of the PCP model. The model is flexible and effective for a variety of MTL-based models.

7. Strengths and Weaknesses:

Strengths:
- The PCP model effectively addresses the issue of obtaining appropriate combination weights in multi-task learning models for e-commerce recommendation systems.
- The proposed approach is motivated by the need for a model that explicitly models personalized combination weights to improve final results, which is a unique and original contribution to the field.
- The PCP model achieves significant improvement in CTR and CVR on a large-scale e-commerce recommendation system and is flexible and effective for a variety of MTL-based models.

Weaknesses:
- The paper lacks a thorough comparison with traditional methods for obtaining combination weights, such as grid search and online A/B tests.
- The proposed approach may not be easily applicable to smaller scale recommendation systems due to the need for a large amount of user data for modeling personalized combination weights.
- The paper could benefit from more detailed explanations and visualizations of the expert network and how it calculates personalized combination weights.
7. Methods: 

- (1): The research methodology proposed in this paper is a personalized combination of predictions (PCP) multi-task learning (MTL) model. The PCP model has a component called the personalized combination expert (PCE) that explicitly models user intention and outputs personalized combination weights. It includes item embedding, user interest embedding, and other context features as inputs to both the PCE and MTL network.

- (2): The PCE is responsible for learning user intention patterns from user history behaviors and outputting personalized combination weights for each user. The PCE is composed of multilayer perceptrons with ReLU activations followed by a softmax layer.

- (3): An alternating training technique is used to effectively update parameters of the expert network and the main MTL network separately. Two loss functions are introduced to supervise the learning of the PCE and MTL, respectively. The loss function for MTL is a weighted sum of the task losses, with hyperparameters manually adjusted according to business considerations. The loss function for the PCE is based on the difference between the predicted output of the main MTL network and the ground truth for each task, multiplied by individual hyperparameters.

- (4): The PCP model achieves significant improvement in click-through rate (CTR) and conversion rate (CVR) compared to traditional MTL models with static combination weights. The proposed approach is motivated by the need for a model that models personalized combination weights to improve final results in industrial recommendation applications. The PCP model is flexible and effective for a variety of MTL-based models.





8. Conclusion:

- (1): This work proposes the Personalized Combination of Predictions (PCP) model, a novel approach to multi-task learning for personalized recommendation in e-commerce. The innovative aspect of the PCP model lies in the use of a personalized combination expert (PCE) component that explicitly models user intention to output personalized combination weights.

- (2): Innovation point: The PCP model introduces a unique and original method to address the issue of obtaining appropriate combination weights in multi-task learning models for e-commerce recommendation systems. Performance: The PCP model achieves significant improvement in click-through rate (CTR) and conversion rate (CVR) on a large-scale e-commerce recommendation system, outperforming state-of-the-art models with static combination weights. The model is also flexible and effective for a variety of multi-task learning-based models. Workload: The paper could benefit from a more detailed comparison with traditional methods for obtaining combination weights and a more comprehensive explanation of the expert network. Additionally, the proposed approach may not be easily applicable to smaller-scale recommendation systems due to the need for a large amount of user data for modeling personalized combination weights.




