# Brain-Tumour-Classification
A few-shot learning approach to brain tumour classification

This project aims to use few-shot learning for brain tumour classification from MRI scans. The
diagnosis of brain tumours can be difficult, so an AI model that can give a second opinion after a doctor
would be very useful. Prototypical learning is the few-shot learning strategy implemented alongside
transfer learning to classify an image given only a few labelled samples of each class. This is relevant as
medical image datasets, such as the brain tumour dataset, are only small and not adequate for training
a full network. This experiment was implemented in Google Colab using Python and used ResNet34
feature extraction. Gaussian noise and masks were applied to the dataset to implement causal learning
and ensure that the model only learned representations from the causal features. The final model was a
3-way, 5-shot design, and many of the hyperparameters had been tuned through different optimisation
methods. The model recorded an accuracy of 97.44% across the test images, which is comparable
to many other designs created in similar research showing the applicability of few-shot learning for
this task. The model could be further improved with a greater analysis of the dataset and improved
fine-tuning methods, as well as a newer version of the ResNet pre-trained model such as ResNet50V2.
