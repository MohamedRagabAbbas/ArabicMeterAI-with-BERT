
# Arabic Poetic Meter Classification with BERT

## Project Overview
This repository contains a detailed Jupyter Notebook (`bert-awzan.ipynb`) which demonstrates the application of the BERT (Bidirectional Encoder Representations from Transformers) model, specifically tailored for the classification of Arabic poetic meters. Using the pre-trained `asafaya/bert-base-arabic` model from Hugging Face's Transformers library, this project exemplifies an advanced NLP technique applied to a unique aspect of Arabic literature.

## Model Details
- **Base Model**: We use `asafaya/bert-base-arabic`, a BERT model that has been pre-trained on a wide range of Arabic texts. This model is well-suited for Arabic language tasks due to its understanding of contextual nuances.
- **Tokenizer**: The accompanying tokenizer for `asafaya/bert-base-arabic` is utilized to ensure that the input text is appropriately pre-processed into a format suitable for BERT.
- **Fine-tuning**: The model is fine-tuned on a labeled dataset comprising various examples of Arabic poetry, where each text snippet is labeled with its corresponding poetic meter. The training involved over 1,900,000 lines of poetry, demonstrating the model's robustness and effectiveness in handling large-scale linguistic data.

## Installation
To replicate the setup and run the notebook on your own machine, follow these steps:
```bash
git clone https://github.com/<your-username>/<your-repository-name>.git
cd <your-repository-name>
pip install -r requirements.txt
```

## Running the Notebook
To execute the notebook and view the project workflow:
```bash
jupyter notebook bert-awzan.ipynb
```

## Example Test Cases
Here are some examples of the test cases used to evaluate the model, showcasing its high accuracy in predicting the correct poetic meters:

| Text                                           | Actual Meter | Predicted Meter |
|------------------------------------------------|--------------|-----------------|
| ماذا أَقول وَفي فَمي                           | الكامل       | الكامل         |
| فَمَتى عَطَستُ فإنّ أنفِيَ أجدعٌ              | الكامل       | الكامل         |
| من الجانبِ الشرقيّ نُوديَ كلُّ مَنْ            | الطويل       | الطويل         |
| كَأَنَّ المِسكَ دُقَّ لَها فَصيغَت             | الوافر       | الوافر         |
| ذو حجرٍ نسبةً وغيظاً                           | البسيط       | البسيط         |

These cases represent a snippet from a larger test set where the model achieved an impressive accuracy of 98.5%, proving its efficacy in the real-world application of classifying Arabic poetic meters.

## Contributing
Contributions are welcome! Here are some ways you can contribute:
- Report bugs and suggest enhancements.
- Add additional test cases.
- Help improve the model's accuracy and efficiency.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Authors
- **Mohamed Abbas**   
 [![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue?style=flat&logo=linkedin)](https://linkedin.com/in/your-linkedin-id)

## Acknowledgments
- Thanks to the developers of the `transformers` library and the creators of the `asafaya/bert-base-arabic` model for providing the tools necessary to undertake this project.
