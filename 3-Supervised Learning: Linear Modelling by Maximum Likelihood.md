# 3-Supervised Learning: Linear Modelling by Maximum Likelihood 最大似然方法

## Linear modelling

* Maps **input attributes** to **output response**;
* **Minimize the loss:** minimize the squared error between model predictions and training observations;
* **Maximize the likelihood:** maximize the likelihood of match between model predictions and training observations;

* **Linear modelling by minimizing loss:** Model shows to capture trend in data observations, but fails to explain each data observation correctly (i.e. error);
* Ignoring error is not right, consider **ERROR as NOISE**.


## Probability

* Joint probability  //联合概率
* Gaussian probability density function  //高斯密度函数
![image](https://github.com/wanyaner/MarkdownPic/blob/master/Gaussian-probability-function.png?raw=true)


## Thinking Generatively 产生式

* Generative model with noise:
![image](https://github.com/wanyaner/MarkdownPic/blob/master/noise-model-function.png?raw=true)

## Maximum Likelihood

1. For each input-response pair(x,t), we have a Gaussian likelihood;
2. Maximize the likelihood of matching all observed responses(t1,t2,...tn) conditioned on the observed data(x1,x2,...xn)and model parameters(w,σ^2);
3. Likelihood & Log() estimate:
![image](https://github.com/wanyaner/MarkdownPic/blob/master/likelihood-estimate.png?raw=true)
4. Finding function's maximum:

![image](https://github.com/wanyaner/MarkdownPic/blob/master/likelihood-w.png?raw=true)and
![image](https://github.com/wanyaner/MarkdownPic/blob/master/likelihood-%CF%83.png?raw=true)

## Model Complexity
* Log() Likelihood:
![image](https://github.com/wanyaner/MarkdownPic/blob/master/log-likelihood-max.png?raw=true)
* **Bias-Variance** tradeoff 偏差－方差的平衡
* Bias:Systematic mismatch; Complex models lead to decrease in bias;
* Variance: more complexmodel has higher Variance.