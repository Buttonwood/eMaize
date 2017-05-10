
https://mlwave.com/kaggle-ensembling-guide/


[Data](http://emaize.imaze.org/emaize/emaize3/emaize_cn.php)


#### 1. 初步想法
父本为国内玉米育种界常用的 30 个优良自交系，母本为 207
个具有广泛变异的自交系。

输入用一个30+207 长度的稀疏向量表示一个输入点;
父本编号前30位,哪一系为1,其他为0;
母本编号后207位,哪一系为1,其他为0;

输出位3长度的向量,即三个性状值

#### 2. 性状和数据分类
1.    female & male 三个性状数据的曲线和分类
2.    genotype做成haplotype(基因型点太多,合并块状)


#### 4.preprocessing
* encoding
    *    0( AA:dominant homozygous)
    *    1( Aa:heterozygous)
    *    2( aa:recessive homozygous)     

#### References
[A machine learning pipeline for quantitative phenotype prediction from genotype data](https://link.springer.com/article/10.1186%2F1471-2105-11-S8-S3)

~~[A Machine Learning Pipeline for Phenotype Prediction from Genotype Data](http://videolectures.net/nipsworkshops09_furlanello_mlpp/)~~

A Monte Carlo Markov Chain model for predicting quantitative traits from genome－wide SNP data

