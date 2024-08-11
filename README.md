# Date Conversion using Sequence-to-Sequence Model with Attention Mechanism

This project illustrates a sequence-to-sequence model with an attention mechanism to transform date formats from a human-readable into a machine-readable one. The primary goal is to train a model that can be potentally used in a machine translation task but doesn't require much computational power. The obtained model accurately converts various date formats into a standardized format, using LSTM networks and an attention mechanism to enhance performance.

## Project Components

- **Data Generation**: The Faker library is used to generate synthetic date data in multiple human-readable formats. These dates are used as inputs. Examples of human-readable date formats include:

*November 22, 2006*

*Tuesday, August 21, 2018*

*Sep 28, 1974*

*1/1/93*

*17 8 1971*

These formats are then transformed into machine-readable formats such as:

*2008-01-23*

*2006-10-22*

- **Building Vocabulary**: The project involves creating vocabularies for both the human-readable and machine-readable date formats.
- **Data Preprocessing**: The generated data is then preprocessed, converting strings into one-hot encodings
- **Model Architecture**: A sequence-to-sequence model is built using an LSTM for the encoder and the decoder, and an attention mechanism to improve the model's focus on relevant parts of the input sequence.
  
## Objectives

- Develop a system that accurately transforms dates from various human-readable formats to a standardized machine-readable format
- Utilize sequence models to enhance the detection accuracy.

## Results

The trained model achieves an accuracy of 0.988 on the test data. The use of an attention mechanism has shown to significantly improve the model's performance.

## References

This code is inspired by the assignment 'Machine Translation' from the Sequence Models course, which is part of the Deep Learning Specialization.
