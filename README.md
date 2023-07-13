#Object detection and boundary boxes

The code in candydetector.py contains the code needed to identify different types of candies. Code is inspired from https://huggingface.co/docs/transformers/tasks/object_detection.

First, labels were made for the images in the "Candy Images" folder using Label Studio, click https://labelstud.io/guide/get_started.html for more information.

The annotated files were then exported, see the "Labelled Data" folder. The result file containing annotation information was converted to to the metadata file found in "Labelled Dataimages" so that it was compatibale with Hugging Face.

"facebook/detr-resnet-50" or "nielsr/detr-resnet-50" model ([https://huggingface.co/docs/transformers/model_doc/](https://huggingface.co/facebook/detr-resnet-50)) could be used to train the model

The model also does inference and counts the number of candies it finds.
