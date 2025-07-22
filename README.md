# Lec3
- Creating LLM = Pre Training + FineTuning

- Pre Training?
training large on diverse dataset
its about understanding human semantics of Questions and Answering
See interaction in chatgpt
How it is able to answer my question?
- why because they trained on huge diverse data

GPT3 - 175Billion data
Datasets Sourses:
Name        Parameters
CommonCrawl 410B
WebText2    19B Reddit Submission Stackoverflow
Book1       12B
Book2       55B
Wikipedia   3B

LLM Pre-trained Predicting next word becuase of that it can do more tasks for example translating
sentiments

Chatgpt: Generate 4 MCQs for egyptian history

it was not specifically trained for that but because it has lot of data it can do it


## FineTuning
- why fine tuning needed?
- Lets say u are manger of airline company
you want to develop chatbot and user want to interact

response you want specific to company but not general answer

Sometimes data is private

you want to develop custom data specific things

its generally called refinement specific to particular task or domain

if you big company and want to deploy their dataset online you need Fine Tuning

for example
SK telecome 
    -related to conversation in Korein
    - they will fine tune GPT-3
    - it will increase accuracy

Harvey.ai
    - AI native legal tool for attorneys and partnered
    - Foundational models (Pre-trained model and data) --> Strongs --> lacks the task specific domains i.e legal case history

JPMorgan Chase unveils AI-powerd LLM suite; may replacce reseach analysit
    - Fine tuned for their employs
 
Production Level you need fineTuning


PreTraining + FineTuning Schematics

Blocks:
    - 1st Data : Internet text book image media research articles
    - 2nd Train : Powerfil GPU requires (GPT 4.6 million dollars) its this much its called Foundational model
    - 3rd FineTuning : trained on label dataset with specific task e.g classification, summarisation, translation, personal assistant

Pretraining :
    - unlabled data we have
    - its kind of forcasting
    - first three words training next word is label.

Steps:
    1. Large Corpus of text data
    Raw means we do not have labels
    2. First training Stage : initial pretraining stage
    3. FineTuning : After obtaining Pretrained LLM's we can further train LLMs on label data.

FineTuning Types

1. Instructional : label dataset instruction-answer pairs e.g text translation, chatbot for customer support

2. Fine Tuning for classification
consist text associated labels
emails spams vs no spams



Big Companies not just use Foundational models but do taskspecific things