# Project: Can you recognize the emotion from an image of a face? 
<img src="figs/CE.jpg" alt="Compound Emotions" width="500"/>
(Image source: https://www.pnas.org/content/111/15/E1454)

### [Full Project Description](doc/project3_desc.md)

Term: Fall 2019

+ Team ##
+ Team members
	+ Zack Abrams zda2105
	+ Kanyan Chen kc3207
	+ Xin Gao xg2298
	+ Chen Wang cw310
	+ Haoyu Zhang hz2563 

+ Project summary: In this project, we created a classification engine for facial emotion recognition. In the original dataset, we have 2500 imgaes and 22 emotions.Here is the data link:[data link](https://www.dropbox.com/s/kvi949ea1rey1d8/train_set.zip?dl=0). For the purpose of imporvment on the accuracy and computational efficiency, we did features extraction at first. Instead of using 6006 ((77*78)/2*2) features, we use 154 features by dropping those highly correlated distances. Furthermore, we remove features with low covariance within emotions and high variance among identity. Then, we train several classification models with training features and responses. We use gbm as our baseline model on selected features and the accuracy we get is 46.2%. Then, the accuracy for random forest model is 45.8%. The accuracy for the svm model is 52%. Thus, we choose svm as our final imporved model. 
	
**Contribution statement**:  Model consturction: Chen Wang, Xin Gao,Kanyan Chen | Features Extraction: Kanyan Chen,Zack Abrams | Github arrangement: Xin Gao, Chen Wang | PPT sturcture: Haoyu Zhang | PPT contex & Presenter: Chen Wang 

Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
