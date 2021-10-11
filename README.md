# Roberta for GoEmotions dataset
- This repo has the hacked up code (goEmotions.ipynb) put together to train the model which is available at the link below:

<b>Trained Model</b>: https://huggingface.co/bsingh/roberta_goEmotion

<b>Dataset</b>: https://huggingface.co/datasets/go_emotions

<b>Original Paper</b>: GoEmotions: A Dataset of Fine-Grained Emotions

<b>Training Details</b>:
- The training script is provided here: https://github.com/bsinghpratap/roberta_train_goEmotion
- Please feel free to start an issue in the repo if you have trouble running the model and I would try to respond as soon as possible.
- The model works well on most of the emotions except: 'desire', 'disgust', 'embarrassment', 'excitement', 'fear', 'grief', 'nervousness', 'pride', 'relief', 'remorse', 'surprise']
- I'll try to fine-tune the model further and update here if RoBERTa achieves a better performance.
- Each text datapoint can have more than 1 label. Most of the training set had 1 label: Counter({1: 36308, 2: 6541, 3: 532, 4: 28, 5: 1}). So currently I just used the first label for each of the datapoint. Not ideal but it does a decent job.
