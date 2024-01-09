# Hackathon Solution Overview

Big thanks to the AI4D Africa’s Anglophone Research Lab for hosting such an amazing hackathon! I appreciate the opportunity to present my solution. Below is a concise guide to help you reproduce my score.

## Steps to Reproduce

1. **Convert Audio Files:**
   - Run the `mp3_to_wav.ipynb` notebook.
   - This notebook facilitates the conversion of audio files from MP3 format to WAV format.

2. **Swahili ASR Implementation: Training+Inference**
   - Execute the `swahili-asr-nemo-Yonas.ipynb` file.
   - This notebook implements the Conformer Large architecture from the Nvidia Nemo toolkit.
   - Specifically, it involves fine-tuning an open-source model obtained from the Hugging Face hub.

3. **Inference with WaV2VeC2-XLSR: Inference alone**
   - Run the `Inference_with_Alamsher.ipynb` file.
   - This standalone notebook can be executed independently.
   - It primarily utilizes the WaV2VeC2-XLSR architecture, performing inference with a model from the Hugging Face hub.

4. **Ensemble ASR Models:**
   - Finally, execute the `Ensemble ASR models.ipynb` file.
   - This notebook combines the csv outputs of the previous two notebooks.

## Submission Details

- **CUDA Devices Used:**
  - GPUs: 1 Nvidia Tesla T4, and 1 Nvidia Tesla P100.

- **Submission File:**
  - Submit the `Ensemble_submission.csv` file, which is the output of the ensemble notebook.


