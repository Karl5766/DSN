# Sparse Network for Time Series Classification: Learning What to “See”


This is the offical implementation for the paper titled Dynamic Sparse Network for Time Series Classification: Learning What to “See”.

## Requirements
- PyTorch 1.4.0
- torchvision 0.2.1
- numpy
- pandas


## Dataset

- The univariate time series datasets (UCR) could be acquired from [here](http://www.cs.ucr.edu/%7Eeamonn/time_series_data/)

- The multivariate time series datasets (UEA) could be acquired from [here](http://www.timeseriesclassification.com/)

- Datasets from UCI could be found [here](https://github.com/titu1994/MLSTM-FCN/releases)

## Training

To train models for **UCR 85 Archive**, change the value of --root (e.g., UCR_TS_Archive_2015) and run this command: 

```
python trainer_DSN.py --sparse True --density 0.2 --sparse_init remain_sort --fix False --growth random --depth 4 --ch_size 47 --c_size 3 --k_size 39

```

To train models for **UCI datasets**, change the value of --root (e.g., UCI) and run this command: 
```
python trainer_DSN.py --sparse True --density 0.2 --sparse_init remain_sort --fix False --growth random --depth 4 --ch_size 47 --c_size 3 --k_size 39

```

To train models for **UEA 30 Archive**, change the value of --root (e.g., UEA_TS_Archive_2018) and run this command: 
```
python trainer_DSN.py --sparse True --density 0.1 --sparse_init remain_sort --fix False --growth random --depth 4 --ch_size 59 --c_size 3 --k_size 39

```

## Other Implementations
The implementation is heavily based on [ITOP](https://github.com/Shiweiliuiiiiiii/In-Time-Over-Parameterization)

## Citation

```
@inproceedings{
xiao2022dynamic,
title={Dynamic Sparse Network for Time Series Classification: Learning What to {\textquotedblleft}See{\textquotedblright}},
author={Qiao Xiao and Boqian Wu and Yu Zhang and Shiwei Liu and Mykola Pechenizkiy and Elena Mocanu and Decebal Constantin Mocanu},
booktitle={Advances in Neural Information Processing Systems},
year={2022},
url={https://openreview.net/forum?id=ZxOO5jfqSYw}
}
```


  
​        
​    
