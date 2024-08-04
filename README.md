# 📝 EmotionFlip Reasoning (EFR) Project

## What is EFR?
In pursuit of this objective, the paper introduces a new challenge named EmotionFlip Reasoning (EFR) in conversational analysis. This task aims to identify all utterances within a dialogue that cause a speaker's emotional state to change. It's important to note that while some emotional shifts may be prompted by other speakers, there are instances where an individual's own utterance can serve as the catalyst for this change.

Formally, the EFR task can be defined as follows:

Let U be a sequence of n utterances [u1, u2, ..., un] in a dialogue conversation D uttered by m distinct speakers [s1, s2, ..., sm]. As the conversation progresses, these speakers express their views or feelings in response to previous utterances. For each utterance ui in the dialogue, there is an associated emotion from the set {anger, fear, disgust, sad, happy, surprise, neutral}, i.e., Ei = fE(ui).

Consequently, if the emotion expressed in utterance ui flips with respect to the speaker's last utterance ul, there might be a set of associated trigger-utterances uk (where 1 <= k <= i) responsible for the emotion-flip, i.e., [..., uk, ...] = fT(ui). In the case of no emotion-flip, a 'non-trigger' label is associated with the current utterance.
![image](https://github.com/user-attachments/assets/06ba9826-a198-4a32-8a17-a521b1921c40)

## 📚 Project Goals
1. Train two models (M3 & M4) with independent architectures different from the one mentioned in the referenced paper. If re-implementing the paper’s model architecture, use the paper’s results as baselines and ensure your scores are comparable.
2. Submit both model checkpoints (M3 and M4) and report the better model with proper reasoning. These models will be tested on the provided testing data during demos.

## 🛠️ Model Setups

### Model M3: Custom Architecture 🧠
- **Description:** A unique model architecture designed for identifying emotion flips within conversations. Details and code are provided in the repository.
![image](https://github.com/user-attachments/assets/9f5b6357-bf3d-4dc1-b2b7-50a0cc41994f)

### Model M4: Custom Architecture 🧠
- **Description:** Another distinct model architecture focusing on the same goals as M3 but with a different approach. Details and code are provided in the repository.
![image](https://github.com/user-attachments/assets/f337d01a-27ba-44fd-b0ca-78865b801b82)


## 📊 Evaluation Metrics
- **Emotion Flip Detection Accuracy**
- **Training and Validation Loss vs. Epochs**

## 📈 Deliverables
1. Model checkpoints for M3 and M4 in proper format.
2. Well-labeled model architectures for both M3 and M4. (If implementing the paper’s model, ignore this deliverable for one model but note the baselines.)
3. Clearly state which of the two architectures performed better and why.
4. A detailed report explaining the intuition behind the models, data splits, and all relevant details.
5. Training loss and validation loss vs. epochs plots for each model.


## 🚀 How to Run
1. **Clone the Repository:**
   ```sh
   git clone <repository-url>
   cd <repository-folder>
