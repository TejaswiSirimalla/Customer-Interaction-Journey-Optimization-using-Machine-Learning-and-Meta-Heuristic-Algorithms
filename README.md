<h1 align='center'>Customer Interaction Journey Optimization using Machine Learning and Meta-Heuristic Algorithms</h1>

**Customer Interaction Journey Optimization using Machine Learning and Meta-Heuristic Algorithms** proposes a way to identify opportunities related to marketing each of a business's products, also considering the products already subscribed, if any, by a customer. Various key factors which help in determining the opportunity are selected. Attributes which could derive these factors are engineered. The likelihood of increase or decrease in these key factors on selling varous products to a customer is forecasted using predictive modeling techniques trained individually to predict each of such likelihood. A weighted aggregate of the predictions made by multiple ML models will be used to determine the opportunities. Metaheuristic algorithm is used to derive a near-optimal journey which maximizes the overall opportunity of the company with the customer.<br><br>
Libraries used: `pandas`, `numpy`, `matplotlib`, `plotly`, `random`, `scikit-learn`, `math`, `joblib`, `os`, `warnings`<br> <br>
Input: <a href = "https://community.ibm.com/community/user/blogs/steven-macko/2019/07/11/telco-customer-churn-1113">IBM's Telco customer churn (11.1.3+)</a> <br>

New features are engineered considering the expertise in the domain and using advise from LLM's. Further, Baye's theorem was used to refine the engineered features. <br>Key factors considered to determine opportunity are CLTV(Customer Life Time Value), Churn Score and Satisfaction Score. The variation in these factors upon purchase of a new product from the business is estimated. The estimations also consider a customer's relationship with the business.<br>

Machine Learning models are trained to predict the features which correspond to variation in the key factors subject to customer's portfolio. Opportunity metic is derived through a weighted combination of these predictions. The distribution of weights among these predictions could be suggested by business based on their requirements. <br>
Simulated annealing is used to fetch a near-optimal journey, among the possible options, constrained by the configurations of various products subscribed by customers.<br> Marketing teams are suggested to utilize the insights derived and communicated from such journeys. An increase in opportunity for retaining a customer could be translated to decrease in risk associated with a customer from being churned. Comparison of decrease in risk from proposed approach with the conventional approaches could be found in the HTML pages from the repository<br>

Link to <a href = "https://drive.google.com/file/d/1S6LqCZte-iccXq7kqXC1QHYmjt1DHkYu/view?usp=drive_link">intermediary files generated during the run</a>. <br>

**Screenshots:**

1. Following plot depects that the risk associated with the journey suggested using proposed approach is least in most of the circumstances than merely considering a journey emphasizing on increase in CLTV.<img width="1037" height="406" alt="Screenshot 2025-10-27 at 3 46 34 AM" src="https://github.com/user-attachments/assets/89aac963-322a-4f71-8698-86520c7c5ab2" />

2. Following plot depects that the risk associated with the journey suggested using proposed approach is least in most of the circumstances than merely considering a journey emphasizing on decrease in Churn Score.
<img width="1040" height="421" alt="image" src="https://github.com/user-attachments/assets/28794d1f-a246-4ec1-9745-062cd5fc59a6" />

3. Following plot depects that the risk associated with the journey suggested using proposed approach is least in most of the circumstances than merely considering a journey emphasizing on increase in Satisfaction Score. <img width="1053" height="426" alt="image" src="https://github.com/user-attachments/assets/e5993aad-0979-4eee-a5d8-4929f168cbf5" />

4. Following plot depects that the risk associated with the journey suggested using proposed approach is least in most of the circumstances than merely considering a journey emphasizing on greedy variations of CLTV, Churn Score and Satisfaction Score.
   <img width="1048" height="426" alt="image" src="https://github.com/user-attachments/assets/8a8a8a09-7f87-476e-8d3e-de9d0c276acc" />

<br>
The notebooks in the repository could be simulated in Kaggle. Interactive graphs for the above plots are saved as HTML files in the repository.
