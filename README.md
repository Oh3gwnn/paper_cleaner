# paper_cleaner

## Download
- Clone this repo:
```bash
git clone https://github.com/hyoungteak/paper_cleaner
cd paper_cleaner
```
- model download:

  https://drive.google.com/file/d/1wGc2FDsIkWCwuVc80BmLMqrdP9WjAuCc/view?usp=sharing

## Requirements
- install the requirements.txt

## Using paper_cleaner
- To cleaning an image use the followng command: 
```bash
python enhance.py ./model_path ./mess_image_path ./directory_to_cleaned_image
```
image:

<img src="https://github.com/min020/paper_cleaner/blob/9bbfb3d7e97b61ea31501b11d904726ef2e856e7/sample/mess_testpaper.png" width="246px" height="290px" alt="testpaper"></img>
<img src="https://github.com/min020/paper_cleaner/blob/9bbfb3d7e97b61ea31501b11d904726ef2e856e7/sample/mess_document.png" width="290px" height="290px" alt="document"></img><br/>

cleaned_image

<img src="https://github.com/min020/paper_cleaner/blob/9bbfb3d7e97b61ea31501b11d904726ef2e856e7/sample/clean_testpaper.png" width="246px" height="290px" alt="testpaper"></img>
<img src="https://github.com/min020/paper_cleaner/blob/9bbfb3d7e97b61ea31501b11d904726ef2e856e7/sample/clean_document.png" width="290px" height="290px" alt="document"></img>

## Training with your own data
- To train with your own data, place your mess images in the folder "data/A/" and corresponding ground-truth in the folder "data/B/". It is necessary that each mess image and its corresponding files are having the same name (could have different extentions), also, the number images  should be the same in both folders.
- Command to train:
```bash
python train.py 
```
- Specifying the batch size and the number of epochs could be done inside the code.

## Reference
- [2022-1H Production log](https://docs.google.com/document/d/1s9Le9lOdZqpJVCQsuTfuk5ucf6vTh2_U_v6xnGVnS2A/edit?usp=sharing)
- [2022-2H Production log](https://docs.google.com/document/d/1w5ktafpL-_PCVLFSW9UmMGo5_DleNonHfOJ1smX0MDw/edit?usp=sharing)
