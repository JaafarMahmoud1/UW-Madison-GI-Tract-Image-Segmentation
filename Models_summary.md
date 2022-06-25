| **Encoder** | **Decoder** | **img_size** | **crop** | **Val_dice** | **Initial-Weights** | **LB_score** | **val_fold** | **TTA** | **epochs** | **DICE LOSS WEIGHT** | **BCE LOSS WEIGHT** | **TEREVSKY LOSS WEIGHT** |
|:-----------:|:-----------:|:------------:|:--------:|:------------:|:-------------------:|--------------|--------------|---------|------------|----------------------|---------------------|--------------------------|
|    Eff_b3   | Nested Unet |      400     |   0.96   |     0.92     |       imagenet      | 87.6         | 0            | Y       | 60         | 0                    | 0.5                 | 0.5                      |
|    Eff_b4   | Nested Unet |      464     |   0.966  |     0.915    |       imagenet      | ??           | 1            | Y       | 60         | 0                    | 0.4                 | 0.6                      |
|    Eff_b4   |     FPN     |      400     |   0.96   |     0.929    |       imagenet      | 87.8         | 2            | Y       | 90         | 1                    | 0                   | 0                        |
|    Eff_b4   |     FPN     |      512     |   0.875   |     0.934    |       imagenet      | 88        | 4            | Y       | 90         | 1                    | 0                   | 0                        |
|    Eff_b5   |     Unet     |      512     |   0.8125   |     0.926    |       imagenet      | 87.6        | 3            | Y       | 120         | 1                    | 0                   | 0                        |
|    Eff_b4   |     FPN     |      512     |   0.875   |     0.934    |       imagenet      | 88.1        | 3            | Y       | 90         | 1                    | 0                   | 0  



## Note:
88.1 model is trained with nearest exact and depth flipped data
