|**ID** | **Encoder** | **Decoder** | **img_size** | **crop** | **Val_dice** |**#slices/centered(forward/backward)** |**reversed** |**Initial-Weights** | **LB_score** | **val_fold** | **TTA** | **epochs** | **DICE LOSS WEIGHT** | **BCE LOSS WEIGHT** | **TEREVSKY LOSS WEIGHT** |
|:-----------:|:-----------:|:-----------:|:------------:|:--------:|:------------:|:------------:|:------------:|:-------------------:|--------------|--------------|---------|------------|----------------------|---------------------|--------------------------|
|0|    Eff_b3   | Nested Unet |      400     |   0.96   |     0.92     |5 - centered|No|       imagenet      | 87.6         | 0            | Y       | 60         | 0                | 0.5                 | 0.5                      |
|8|    Eff_b4   | Nested Unet |      464     |   0.966  |     0.915    |5 - centered|No|       imagenet      | ??           | 1            | Y       | 60         | 0                | 0.4                 | 0.6                      |
|9|    Eff_b4   |     FPN     |      400     |   0.96   |     0.929    |5 - centered|No|       imagenet      | 87.8         | 2            | Y       | 90         | 1                | 0                   | 0                        |
|15|    Eff_b4   |     FPN     |      512     |   0.875   |     0.934    |7 - centered|No|       imagenet      | 88        | 4            | Y       | 90         | 1                | 0                   | 0                        |
|13|    Eff_b5   |     Unet     |      512     |   0.8125   |     0.926    |7 - centered|No|       imagenet      | 87.6        | 3            | Y       | 120         | 1            | 0                   | 0                        |
| ?|    Eff_b4   |     FPN     |      512     |   0.875   |     0.934    |?|?|       imagenet      | 88.1        | 3            | Y       | 90         | 1              | 0                   | 0  
|21|    Eff_b4   | DeepLabV3+  |      512     |   0.875   |     ?        |7 - centered|Yes|       imagenet      | 88.1        | 4            | Y       | 90         | 1                  | 0                   | 0  
|19|    Eff_b4   |     FPN     |      544     |   0.882   |     ?    |7 - centered|Yes|       imagenet      | 88.1       | 4            | Y       | 90         | 1                    | 0                   | 0 



## Note:
88.1 model is trained with nearest exact and depth flipped data
