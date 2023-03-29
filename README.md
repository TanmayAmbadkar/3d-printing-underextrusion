# Early detection of 3D printing issues

## Goal of this competition
3D printing is an innovative way to fabricate parts from any 3D geometry model. However, 3D printing is also known to be prone errors. Most of these errors are visible via a close-up camera mounted right near the printer nozzle.

The goal of this competition is to predict 1 specific kind of error - under extrusion.

## Attempts

I have tried the following 3 methods:

1. ViT Finetuning - Finetuning ViT on the dataset directly
2. ViT Contrastive learning - Using contrastive learning as a pretraining task for a custom ViT and finetuning for classification
3. Bagging - Dividing an image into 4 regions and using 4 predictions for making a final prediction.
