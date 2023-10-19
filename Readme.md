# Shore Livecams: A Maritime Dataset for Deep Learning based Object Detection
A maritime dataset for object detection. The dataset is a collection of high definition (HD), full high definition (FHD), ultra high definition (UHD) images captured from live video feeds recorded across various port based areas of Germany. These images contain multiple instances of objects which are primarily classified into three different classes and annotated accordingly.

Prepaired to be used with YOLO PyTorch implementations.

## Label formats
Labels are provided in folloing formats:
* YOLO
* PascalVOC .xml (Foldername: train_voc)
* COCO .json

## Folder structure
The folder structure looks like this:
```
images/
    test/
        2ux5cw8z_1080_2022-07-16_11-26_output_0.jpeg
        ...
    train/
        2ux5cw8z_1080_2022-07-17_02-54_output_0.jpeg
        ...
labels/
    test/
        2ux5cw8z_1080_2022-07-16_11-26_output_0.txt
        ...
    test_voc/
        2ux5cw8z_1080_2022-07-16_11-26_output_0.xml
        ...
    train/
        2ux5cw8z_1080_2022-07-17_02-54_output_0.txt
        ...
    train_voc/
        2ux5cw8z_1080_2022-07-17_02-54_output_0.xml
        ...
    shore_livecams.yaml # YOLO v5 PyTorch dataset file for dataloader
    train.json
    test.json
    train+test.json
```

## Dataset Statistics
* 3 classes [human, land, sea]
* 17,6 objects per image average
* Image resolution: 
    * 720p (116)
    * 1080p (392)
    * 3840p (17)

Distribution in total, train and test
|       | images | objects | human | land | sea  |
|-------|--------|---------|-------|------|------|
| total | 525    | 9243    | 2821  | 3378 | 3044 |
| train | 394    | 5643    | 1624  | 1976 | 2043 |
| test  | 131    | 3600    | 1197  | 1402 | 1001 |

## Citation
If you find this dataset helpful, please cite this paper (to be published):

D. Ahlers, P. Bhattacharya, P. Nowak, and U. Zölzer, "Shore Livecams: A Maritime Dataset for Deep Learning based Object Detection", in 17th International Conference on Signal Image Technology & Internet based Systems (SITIS), 2023.