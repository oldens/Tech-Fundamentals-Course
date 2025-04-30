# Lesson 2: Probability for ML: Bayes' Theorem

## Topics
- Basics of probability theory
- Conditional probability
- Bayes' theorem
- Examples of application in classification

## Notes
Probability theory is a branch of mathematics that deals with the analysis of random events. It provides the foundation for many machine learning algorithms, especially those involving uncertainty and prediction.

### Basics of Probability Theory
1. **Probability**: A measure of the likelihood that an event will occur.
2. **Random Variable**: A variable whose possible values are numerical outcomes of a random phenomenon.
3. **Probability Distribution**: A function that describes the likelihood of different outcomes.

### Conditional Probability
Conditional probability is the probability of an event occurring given that another event has already occurred. It is denoted as P(A|B), which reads as "the probability of A given B".

### Bayes' Theorem
Bayes' theorem describes the probability of an event based on prior knowledge of conditions that might be related to the event. It is expressed as:

\[ P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)} \]

Where:
- \( P(A|B) \) is the posterior probability: the probability of event A occurring given that B is true.
- \( P(B|A) \) is the likelihood: the probability of event B occurring given that A is true.
- \( P(A) \) is the prior probability: the initial probability of event A.
- \( P(B) \) is the marginal probability: the total probability of event B.

### Examples of Application in Classification
Bayes' theorem is widely used in classification problems, such as spam detection in emails. By calculating the probability that an email is spam based on the presence of certain words, we can classify emails more accurately.

For example, if we want to determine whether an email is spam (S) or not spam (¬S) based on the presence of the word "offer" (O), we can use Bayes' theorem:

\[ P(S|O) = \frac{P(O|S) \cdot P(S)}{P(O)} \]

By calculating these probabilities, we can make informed decisions about the classification of emails.
