# HWxPI Track at 2018 ICPR Multimedia Information Processing for Personality & Social Networks Analysis Challenge

## Task description

The tasks consist in estimating the personality traits of users from their handwritten texts and the corresponding transcripts (see the dataset description above). The challenge comprises two phases, development and final phases. For the first phase, the participants should develop their systems using a set of development pairs of handwritten essays (including image and text) from 418 subjects. Each subject has an associated class 1 and 0, corresponding to the presence of a high pole or a low pole of a specific personality trait. The traits correspond to the Big Five personality model used in psychology: Extraversion, Agreeableness, Conscientiousness, Emotional stability, and Openness to experience. Thus, participants will have to develop a classifier to predict the pole of each trait, this classifier should be able to use the information from both modalities (i.e. textual and visual). For the final evaluation phase, an independent set of 293 unlabeled samples will be provided to the participants, who will have to provide predictions using the models trained on development data. The winners of the challenge will be determined with basis on the final phase performance.

The corpus used in this task consists of handwritten Spanish essays from undergraduates Mexican students. For each essay two files are available: a manual transcript of the text and a scan image of the original sheet where the subject hand-wrote the essay. The texts of manual transcriptions have tags to mark some handwritten phenomena namely: <FO:well-written word> (misspelling), <D:description> (drawing), <IN> (insertion of a letter into a word), <MD> (modification of a word, that is a correction of a word), <DL> (elimination of a word), <NS> (when two words were written together; e.g. Iam instead of I am) and, SB (syllabification). Figure 2 below shows a pair of essays with their corresponding image and text. Each essay is labelled with five classes corresponding to five personality trait in the Big Five Model of Personality. The traits are Extraversion, Agreeableness, Conscientiousness, Emotional stability, and Openness to experience. The classes for each trait are 1 and 0 corresponding to the high pole and low pole of each trait, respectively. To assign each label in the dataset we use an instrument named TIPI (Ten Item Personality Inventory), this instrument includes a specific set of norms for each trait.

The HWxPI Track is running under the CodaLab platform. To access the task follow this link (click on the link).

The track is organized in two phases as follows:

- Phase 1: Labeled development and unlabeled validation data is made available to participants. During this phase, participants can train their models using development data and submit predictions on validation data to the CodaLab site: https://competitions.codalab.org/competitions/18362 . Participants will receive immediate feedback that will be displayed in the leaderboard.
- Phase 2: Participants will have access to unlabeled test data, and they should submit predictions of their systems to the CodaLab site. Performance in this test partition will be used to determine the winners.

## Dataset description

#### HWxPI Handwritten texts for Personality Identification Dataset

The HWxPI data set used in this task consists of handwritten Spanish essays from undergraduates Mexican students. For each essay two files are available: a manual transcript of the text and a scan image of the original sheet where the subject hand-wrote the essay. The texts of manual transcriptions have tags to mark some handwritten phenomena namely: FO (the previous word is misspelled), D (there is a drawing here; e.g. an emoji, a signature, etc), <IN> (insertion of words into the text), <MD> (modification of a word, that is a correction of a word; e.g. when the subject forgot to write a letter and modified the word), <DL> (elimination of a word), <NS> (when two words were written together; e.g. Iam instead of I am) and, SB (syllabification). Each essay is labelled with five classes corresponding to five personality trait in the Big Five Model of Personality. The traits are Extraversion, Agreeableness, Conscientiousness, Emotional stability, and Openness to experience. The classes for each trait are 1 and 0 corresponding to the high pole and low pole of each trait, respectively. To assign each label in the dataset we use an instrument named TIPI (Ten Item Personality Inventory), this instrument includes a specific set of norms for each trait.

Files ending in .data contain 3 columns, the first corresponds to the subject’s id, the second contains the path for the transcript file (i.e., a text file), and the last column contains the path for the transcript’s image (i.e., an image file) of that instance.

Each row in the .data file correspond to the same row in the .solution file for both the training and validation set. The order of traits in the .solution columns are: EXT AGR CON STA OPE; where each code stands for extraversion, agreeableness, conscientiousness, emotional stability and openness, respectively.

## Evaluation metrics

As described previously, the problem of personality recognition consists in a binary classification problem for each of five traits. Thus, the evaluation of the participants teams will be through standard set-based metrics, such as F-measure, accuracy, and the the ROC AUC measure. The leading evaluation measure for ranking participants is the macro averaged Area Under the ROC Curve (auc_multilabel)

Originally posted in [ChaLearn Looking at People](http://chalearnlap.cvc.uab.es/challenge/27/description/).

# Cite:

Ramírez, Gabriela, et al. “Overview of the Multimedia Information Processing for Personality & Social Networks Analysis Contest.” Pattern Recognition and Information Forensics, edited by Zhaoxiang Zhang et al., Springer International Publishing, 2019, pp. 127–39. Springer Link, doi:10.1007/978-3-030-05792-3_12.
