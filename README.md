# EmoEd: Multimodal Emotion-Cause Pair Extraction in Conversations
## DS510 : Artificial Intelligence and Machine Learning Lab Course Project

### Team Members:
1. **Ganta Naga Jaswanth**
2. **Chelluboina Siri**

### Project Description:
EmoEd is the course project for the Artificial Intelligence and Machine Learning Lab Course. The project aims to extract emotion-cause pairs from the conversations. The project is based on the paper [Multimodal Emotion-Cause Pair Extraction in Conversations](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9969873).

Objective is extracting emotion-cause pairs from conversational data using multimodal signals such as text, audio, and video. The goal is to predict emotions expressed in conversations and identify corresponding causes by leveraging deep learning models like BiLSTM and BERT.

Features
- Multimodal Analysis: Integrates text, audio, and video data for comprehensive emotion and cause detection.
- Emotion-Cause Pair Extraction: Identifies pairs of emotions and their causes within conversations.
- Deep Learning Models: Utilizes BiLSTM for sequence classification tasks.

### Dataset:
We use the ECF dataset, which is a multimodal dataset for emotion-cause pair extraction in 'Friends' sitcom. The dataset contains over 13,000 annotated emotion-cause pairs from 1,374 conversations in the 'Friends' sitcom. The dataset includes text, audio, and video data for each conversation along with emotion labels and cause annotations.

### Methodology:
Refer to [report](EmoEd_Report.pdf) for detailed methodology.

### Results:
Refer to [report](EmoEd_Report.pdf) for detailed results.

### Installation:

#### Pre-requisites:
- Python 3.11
- pip3

#### Setup:
1. Clone the repository
```bash
git clone https://github.com/nagajas/EmoEd.git
cd EmoEd
```

2. Create a virtual environment (optional)
```bash
python3 -m venv venv
source venv/bin/activate
```

3. Install the dependencies
```bash
pip install -r requirements.txt
```

### Usage

To train the BiLSTM model for emotion and cause extraction, run:

```bash
python BiLSTM_EC.py
```
After training, extract emotion-cause pairs by running:

```bash
python pair.py
```
### Project Structure
- [BiLSTM_EC.py](./BiLSTM_EC.py): Script for training the BiLSTM model for emotion and cause utterance extraction.
- [pair.py](./pair.py): Script for predicting emotion-cause pairs using the trained model.
- [data](./data): Directory containing the ECF dataset.
- [feature_extraction](./feature_extraction): Contains feature extraction scripts.
- [helper.py](./helper.py): Utility functions.
- [requirements.txt](./requirements.txt): Python dependencies.

### Deployment Interface
Visualizing Emotion Cause relation for a test conversation from th ECF.
![Deployment](./assets/deploy.png)

For more details, refer to the [report](EmoEd_Report.pdf).