# COVID-19 Detection using Chest X-Ray Images
[Download trained model](https://drive.google.com/file/d/1EcEGBdNsbolGXls2tdEJyv6UpEAEGhze/view?usp=sharing)

![covid-predictor](https://github.com/user-attachments/assets/ba841fb5-f1c8-4030-9352-660c186c7ec9)

This Jupyter notebook demonstrates the process of predicting the possibility of COVID-19 in a patient by training a machine learning model. The dataset used for this project is a collection of chest X-ray images from the University of Montreal, available on Kaggle.

## Dataset

The dataset can be found [here](https://www.kaggle.com/datasets/pranavraikokte/covid19-image-dataset/data). It contains images categorized into three classes:
- COVID-19
- Normal
- Viral Pneumonia

## Classification Report

The classification report generated after training the model is as follows:

```
                 precision    recall  f1-score   support

          covid       1.00      0.96      0.98        26
         normal       0.83      0.75      0.79        20
viral pneumonia       0.74      0.85      0.79        20

       accuracy                           0.86        66
      macro avg       0.86      0.85      0.85        66
   weighted avg       0.87      0.86      0.87        66
```

## Training Logs

The model was trained for 35 epochs. Below are the training logs for each epoch:

```
Epoch 1/35
8/8 ━━━━━━━━━━━━━━━━━━━━ 3s 299ms/step - accuracy: 0.3656 - loss: 1.1402 - val_accuracy: 0.6818 - val_loss: 1.0421
Epoch 2/35
8/8 ━━━━━━━━━━━━━━━━━━━━ 2s 292ms/step - accuracy: 0.5516 - loss: 1.0247 - val_accuracy: 0.8182 - val_loss: 0.7128
...
Epoch 34/35
8/8 ━━━━━━━━━━━━━━━━━━━━ 2s 294ms/step - accuracy: 0.8701 - loss: 0.3192 - val_accuracy: 0.8939 - val_loss: 0.3092
Epoch 35/35
8/8 ━━━━━━━━━━━━━━━━━━━━ 3s 303ms/step - accuracy: 0.8619 - loss: 0.3588 - val_accuracy: 0.8636 - val_loss: 0.3330
```

## Conclusion

This notebook provides a comprehensive workflow for training a CNN to detect COVID-19 from chest X-ray images. The model achieves an overall accuracy of 86% and performs particularly well in identifying COVID-19 cases.

For further improvements, consider experimenting with different model architectures, data augmentation techniques, and hyperparameter tuning.

## Acknowledgements

- Dataset: [COVID-19 Image Dataset](https://www.kaggle.com/datasets/pranavraikokte/covid19-image-dataset/data) by Pranav Raikokte on Kaggle.
