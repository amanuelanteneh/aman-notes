# Machine Learning


Broadly speaking the problem of machine learning can be stated as {cite:p}`james2023statistical`: 

We are given a set of data points $\mathcal{X}$ in some $p$-dimensional space i.e. a set of predictor variables $X=(X_1, \dots X_p)$ and a quantitative response variable $Y$. We _assume_ there is some relationship between the response and the predictors which can be written as 

$$ Y = f(X) + \varepsilon $$

where $f(X)$ is a function of the $p$ predictors and $\varepsilon$ is a random variable (error/noise term) with $\mathbb{E}(\varepsilon)=0$ and $\textrm{Var}(\varepsilon)=\sigma_\varepsilon^2$. This $\varepsilon$ is the source of what is called _irreducible error_.  Generally the problem of machine learning is to find an estimate $\hat{f}(X)$ of $f(X)$ given the set of data points $\mathcal{X}$ that we assume come from the function $Y = f(X)+\epsilon$.