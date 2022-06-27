# Semantic segmentation

## Changes done to obtain the score 881:
### from training side:
* NEAREST_EXACT resize
* Eff b4 with FPN
* Train for 90 epochs
* Dice loss only

### from inference side:
* NEAREST_EXACT resize
* H flip TTA
* classify empty masks using max pixel probability

## Info about the best submission
- Ensemble of 6 models (3 trained with 5 slices and 3 trained with 7 slices)
- Models differs in Image size - crop ratio - encoders and decoders
- Best 5 slices Model score is .878
- For more infor about the models <a href="https://github.com/JaafarMahmoud1/UW-Madison-GI-Tract-Image-Segmentation/blob/Best_single_model/Models_summary.md">see</a>
- One model of 7 slices trained with depth flip  

## tried but didn't work:
- Upscaling TTA
- Train a model that will take slices in between (-4 -2 0 2 4) instead of (-2 -1 0 1 2) to cover the difference between adults and childs
- Remove masks with BBOXES smaller than 7X7
