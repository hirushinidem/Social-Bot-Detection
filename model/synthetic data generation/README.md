The initial dataset exhibited a significant class imbalance, with 129,856 human (non-bot) tweets and 4,342 bot tweets. This severe imbalance, where bot tweets represented only about 3.2% of the total data, could potentially lead to poor model performance in detecting bot accounts. To address this imbalance, synthetic bot data was generated to increase the minority class, resulting in a more balanced distribution. The final dataset, contained 129,856 non-bot tweets (0.0) and 104,342 bot tweets (1.0), achieving a more balanced ratio of approximately 55% to 45%. This approach of synthetic data generation was chosen over traditional sampling methods to maintain the authentic characteristics of human tweets while creating realistic bot patterns, ultimately providing the model with sufficient examples of both classes for effective learning.
The synthetic data generation process significantly improved the class balance by augmenting the original bot class (class 1.0). Starting with only 4,342 real bot tweets, synthetic data generation created approximately 100,000 additional bot examples using carefully crafted methods from the code. The process involved:
1.	Using the Faker library to generate tweet content with realistic text patterns
2.	Incorporating specific bot-like features:
3.	Extracting meaningful features for each synthetic tweet: 
I.	Number of mentions (@) and hashtags (#)
II.	Percentage of organizational references
III.	Percentage of person references
IV.	Always labeled as bot (1.0)
The generation process increased the bot class from 4,342 to 104,342 instances, while maintaining the original 129,856 human tweets. This resulted in a near-balanced final distribution (55% human vs 45% bot), making the dataset more suitable for training an unbiased bot detection model.
