# Human-Centered-Machine-Learning
This is a project for the HCML course at UU titled: **Counterfactual Fairness Analysis for Credit Default**.

### Abstract
This project investigates fairness in credit default prediction using an interpretable logistic regression model and counterfactual explanations.
We evaluate a credit default classifier trained on the UCI "Default of Credit Card Clients" dataset, focusing on fairness across demographic groups such as gender, age, and marital status.
Standard group fairness metrics are first computed to assess disparities in model outcomes.
To complement this, we implement an effort-based counterfactual analysis that quantifies how much individuals must change their actionable features to reverse an unfavorable outcome while keeping protected attributes constant.
While standard fairness metrics showed that the model favours females, our counterfactual analysis indicated that the model helps males.
Specifically, while it is more likely for the model to predict 'default' (unfavourable outcome) for males, our counterfactual analysis showed that when females are predicted to default, it is more difficult for them, although not significantly, to change their outcome to a favourable one.
This confirms that fairness is multidimensional.
Even when prediction rates appear in favor of one group (in this case, females are in favor based on standard fairness metrics), the effort for changing to a favourable outcome might also be higher for this group (in this case, females require more effort in changing their outcome to 'no default').
Therefore, evaluating fairness using only standard fairness metrics (such as statistical parity or TPR) may overlook disparities embedded in the model’s behavior.
