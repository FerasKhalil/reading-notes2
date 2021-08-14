# Read: Class 16 Machine Learning Intro

## Data Science Primer

### Bird's Eye View
- machine learning is not about algorithms
- Machine learning is a comprehensive approach to solving problems
- Machine learning is the practice of teaching computers how to learn patterns 
	from data, often for making decisions or predictions.


- **Example: the curious child** 
A young child is playing at home... And he sees a candle! He cautiously waddles over.

Out of curiosity, he sticks his hand over the candle flame.
"Ouch!," he yells, as he yanks his hand back.
"Hmm... that red and bright thing really hurts!"
Ooh a candle!
Ooh a candle!

Two days later, he's playing in the kitchen... And he sees a stove-top! Again, he cautiously waddles over.

He's curious again, and he's thinking about sticking his hand over it.
Suddenly, he notices that it's red and bright!
"Ahh..." he thinks to himself, "not today!"
He remembers that red and bright means pain, and he ignores the stove top.
To be clear, it's only machine learning because the child learned patterns from the candle.

He learned that the pattern of "red and bright means pain."
On the other hand, if he ignored the stove-top simply because his parents warned him, that'd be "explicit programming" instead of machine learning.

	- [Example from](https://elitedatascience.com/birds-eye-view)



### Exploratory Analysis
- The purpose of it is to get to know the  dataset. doing so upfront  will make the rest of the project much smoother in 3 ways.
1. gain valuable hints for data cleaning
2. think of ideas for future engineering
3. help you communicate results and dilever greater impact.

#### plots
1. Plot Categorical Distributions:
	- Categorical features cannot be visualized through histograms. Instead, you can use bar plots.
		- [source from](https://elitedatascience.com/exploratory-analysis)
2. Plot Segmentations
	- Segmentations are powerful ways to observe the relationship between categorical features and numeric features.
		- [source from](https://elitedatascience.com/exploratory-analysis)

### Data Cleaning
- First step is to remove unwanted observations from your dataset
	- like duplicates or irrelevant obserations
- fix structural errors like typos
- filter unwanted outliers



### Feature Engineering
- Feature engineering is about creating new input features from your existing ones.
	- [source from](https://elitedatascience.com/feature-engineering)
#### Infuse Domain Knowledge
- You can often engineer informative features by tapping into your (or others’) expertise about the domain.
	- [source from](https://elitedatascience.com/feature-engineering)

#### Combine Sparse Classes
- Sparse classes (in categorical features) are those that have very few total observations. They can be problematic for certain machine learning algorithms, causing models to be overfit.
	- [source from](https://elitedatascience.com/feature-engineering)

#### Remove Unused Features
- Unused features are those that don’t make sense to pass into our machine learning algorithms.
	- [source from](https://elitedatascience.com/feature-engineering)


### Algorithm Selection
#### Tree Ensembles
- Ensembles are machine learning methods for combining predictions from multiple separate models. There are a few different methods for ensembling, but the two most common are:
	1. Bagging
	2. Boosting
		- [source from](https://elitedatascience.com/algorithm-selection)

### Model Training

#### Model Training
Think of your data as a limited resource.

- You can spend some of it to train your model (i.e. feed it to the algorithm).
- You can spend some of it to evaluate (test) your model.
- But you can’t reuse the same data for both!
	- [source from](https://elitedatascience.com/model-training)


#### Hyperparameters
-  it's tuning models