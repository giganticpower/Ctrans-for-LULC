# From CATrans: Remote Sensing Image Segmentation based on Cross Scale Attention and Visual Transformer
[From CATrans: Remote Sensing Image Segmentation based on Cross Scale Attention and Visual Transformer]
## Abstract
CATrans: Remote Sensing Image Segmentation based on Cross Scale Attention and Visual Transformer
## Method

## Test and train
Our code is based on [GLNet](https://github.com/VITA-Group/GLNet)  
python>=3.6 and pytorch>=1.2.0  
Please install the dependencies: `pip install -r requirements.txt`
### dataset
Please register and download [Inria Aerial](https://project.inria.fr/aerialimagelabeling/) dataset  
Create folder named 'data_1', its structure is  
```
data_1/
├── train
   ├── Sat
      ├── xxx_sat.tif
      ├── ...
   ├── Label
      ├── xxx_mask.png(two values:0-1)
      ├── ...
├── crossvali
├── offical_crossvali
```
### test
`bash test.sh`  
### train
Please sequentially finish the following steps:   
1.`bash train_pre.sh`(not necessary)  
2.`bash train_B10.sh`(get medium context)  
3.`bash train_B15.sh`(get large context)  
4.`bash train.sh`  

## Citation
our paper will be released soon.
