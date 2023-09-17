# Facial_Emotion_Recognition_Using_DL


This project involves fine-tuning a pre-trained emotion recognition model using a custom dataset and utilizing the fine-tuned model for real-time emotion detection from a webcam feed.

## Overview

The main components of this project include:

1. **Fine-Tuning the Model**: The provided code demonstrates how to fine-tune a pre-trained model using a custom dataset of emotion-labeled images. The fine-tuned model is saved as 'Facial_Recognition_fine_tuned.h5' for future use.

2. **Real-Time Emotion Detection**: The code allows you to use the fine-tuned model for real-time emotion recognition from a webcam feed. Detected emotions are displayed as labels on the video stream.

## Fine-Tuning the Model

1. Place your preprocessed dataset in the 'Face_emotions' directory with the following structure:

   ```
   - Face_emotions/
     - train/
       - emotion1/
         - image1.jpg
         - image2.jpg
         ...
       - emotion2/
         - image1.jpg
         - image2.jpg
         ...
     - test/
       - emotion1/
         - image1.jpg
         - image2.jpg
         ...
       - emotion2/
         - image1.jpg
         - image2.jpg
         ...
   ```

2. Run the fine-tuning code provided in your project's Python environment. This code loads the pre-trained 'best_model.h5', fine-tunes it using the dataset, and saves the fine-tuned model as 'Facial_Recognition_fine_tuned.h5'.

## Usage - Real-Time Emotion Detection

To use the fine-tuned emotion recognition model for real-time emotion detection:

1. Load the fine-tuned model:

   ```python
   from tensorflow.keras.models import load_model

   emotion_model = load_model('Facial_Recognition_fine_tuned.h5')
   ```

2. Initialize the webcam feed:

   ```python
   import cv2

   cap = cv2.VideoCapture(0)
   ```

3. Run the real-time emotion detection code:

   ```python
   # [Insert real-time emotion detection code here]
   ```

4. Close the webcam feed and OpenCV windows by pressing 'q'.

Ensure you have the required libraries installed using `pip install tensorflow opencv-python`.

## Additional Information

- The fine-tuned model can be further integrated into other applications for emotion recognition from images or video streams.

- Modify the emotion labels and recognition logic according to your dataset and requirements.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- TensorFlow and Keras communities for providing deep learning tools and resources.

## Contact

For any questions or feedback, please contact [Ramanand R](mailto:ramanandr786@outlook.com).

---
