# LLM Model Parameters

[Go Back](/main.md)

LLM Parameters are settings that you can adjust to control how the LLM generates texts. They can affect the quality, diversity, and creativity of the generated texts. Some of the common LLM parameters are temperature, number of tokens, top-p, presence penalty, and frequency penalty.

## Temperature

Temperature is a parameter that controls how much randomness is introduced in the text generation process. A higher temperature means more diversity and unpredictability, while a lower temperature means more coherence and consistency.

## The number of tokens

The number of tokens is a parameter that controls how long the generated text is. A higher number of tokens means more detail and information, while a lower number of tokens means more conciseness and simplicity.

## Top-P

Top-p is a parameter that controls how many words are considered candidates for the next word in the text generation process. A higher “Top-p” means more diversity and creativity, while a lower “Top-p” means more accuracy and reliability.

## Presence Penalty:

Presence penalty is a parameter that controls how much the generated text reflects the presence of certain words or phrases in the output text so far. A higher “presence penalty” encourages the model to explore new topics and makes it less repetitive, while a lower “presence penalty” means more repetition and less exploration.

As we can see, the “presence penalty” parameter penalizes the model when reusing tokens that have appeared in the output text so far, regardless of whether they are in the prompt or not. You can use different presence penalty values depending on your purpose and preference.

- Presence penalty = 0.0: The best sport is soccer, soccer, soccer. This is a - very repetitive and emphatic text, but also very boring and monotonous.
- Presence penalty = 0.5: The best sport is soccer, basketball, and tennis. This is a more varied and novel text, but still somewhat coherent and consistent.
- Presence penalty = 1.0: The best sport is soccer, rugby, and chess. This is a very varied and novel text, but also very diverse and unpredictable.

## Frequency Penalty:

Frequency penalty works the same way the Presence penalty works but it includes tokens present in the prompt when applying the penalty.It scales based on how many times that token has appeared in the text so far including the prompt. So, a token that has already appeared more times gets a higher penalty and then this token has less probability of appearing.

To illustrate this, let’s imagine a LLM generating some texts based on the same prompt: “The best sport is soccer”. I will use different “frequency penalty” values and see how the texts change. Here are some examples:

- Frequency penalty = 0.0: The best sport is soccer**, soccer is fun, and soccer is exciting.** This is a very repetitive and emphatic text, but also very boring and monotonous.
- Frequency penalty = 0.5: The best sport is soccer**, soccer is fun and exciting.** This is a more varied and novel text with less repetitions, but still somewhat coherent and consistent.
- Frequency penalty = 1.0: The best sport is soccer**, football is fun and exciting.** This is a very varied and novel text, but also very diverse and unpredictable, notice that it didn’t repeat the word “soccer” present in the prompt.

[Source](https://michaelehab.medium.com/the-secrets-of-large-language-models-parameters-how-they-affect-the-quality-diversity-and-32eb8643e631)
