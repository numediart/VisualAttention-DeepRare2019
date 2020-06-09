# DeepRare2019 (DR2019)
Rarity is computed on the deep features extracted by a VGG16 trained on ImageNET. No training is needed. This model is neither "feature engineered saliency model" as features come from a DNN model, nor a DNN-based model as it needs no training eye-tracking dataset. It is thus a "deep-engineered" model. Just apply it one your images. A full paper can be found here : [https://arxiv.org/abs/2005.12073](https://arxiv.org/abs/2005.12073).
If you use DR2019, please cite :   
  
>`@misc{matei2020visual,  
 title={Visual Attention: Deep Rare Features}, author={Mancas Matei and Kong Phutphalla and Gosselin Bernard}, year={2020}, eprint={2005.12073}, archivePrefix={arXiv}, primaryClass={cs.CV}}`  

### How to run

Just type :

```python
>>python run_DR_2019.py
```

The main function takes in a folder all the images, show results and record the saliency map in a different folder. 

### Paper results reproduction

The result from this code is the raw data which will not let you reproduce exactly the paper results. For this purpose you still need to low-pass filter the results and, for natural images datasets (such as MIT1003 ...), add also a centred Gaussian. For O3 and P3 datasets, centred Gaussian is not used. 
The codes used for smoothing and adding centred Gaussian are the Matlab codes from the MIT benchmark website. This website moved to Tubingen and the tools might have changed a little. 

### Requirements

The codes were tested with the following configuration: 

* Python 3.6.10
* Numpy 1.11.6
* OpenCV 4.1.2
* Keras 2.2.0
* Tensorflow 1.5.0
* Matplotlib 3.1.2

### Licence

This code is free to use, modify or integrate in other projects if the final code is for research and non-profit purposes and if our paper is cited in the code and any publication based on this code. This code is NOT free for commercial use. For commercial use, please contact matei.mancas@umons.ac.be 

### Waranty

This code is provided 'as is' with no waranty or responsability from the authors or their institution. 

### Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

‎ 
