# Few-shot fish recognition CNN model with Pytorch
Recognition of fish species with stable accuracy and high efficiency is important for observation of fish population quantity and governing of ecological environment at their habitats. As most of fishes are wildlife, the collection of their images can be hard, so traditional deep learning methods, which relies on large labeled datasets is limited while doing such works. 

Few-shot is a rising method in deep learning image recognition. By imitating human, who use prior knowledge to remember new things, it can learn the common process of classes detection using image. Therefore, it is able to know how to detect the label right after seeing a few samples of a new class. Due to this advantage, few-shot methods significantly reduce the cost of data acquirement and labeling, as well as its strong generalization ability, which is very suitable in fish species detection.

This project proposed a new few-shot model, which uses ResNet as backbone. I firstly used mini-ImageNet to pre-train the model, and move its parameters under transfer learning condition. Then, used the Fish100 dataset, a fish image dataset which is a subset of Image CLEF, to train and test this model, and made a contrast with other 5 kinds of current models. The result shows that the new model has reached the best performance of 0.9084, along with a better precision, recall, and F than all other models.

The mini-ImageNet and Fish100 dataset is zipped in 'materials.zip', to use them please unzip it first.

Folder 'save' contains previous trained models, it can be used directly with model.upload().
