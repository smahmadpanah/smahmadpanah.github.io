---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<script>
  $(document).ready(function () {
    $(".abstract").hide();
    $(".button").on("click", function () {
        $(this).next(".abstract").slideToggle(400);
    });
});
</script>


<style>
.abstract{text-align:justify; }
.button{ text-align:justify; }
</style>

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}



<ol reversed>

<div id="7">
<li> <b>Entri: Ensemble Learning with Tri-Level Representations for Explainable Scene Recognition - Pattern Recognition in review process</b> [<a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4482110">Link</a>]
<br><i>Amirhossein Aminimehr</i>, Amirali Molaei, and Erik Cambria
<div class='button' data-content="toggle-text"><a href="#7">abstract</a></div>
<div class='abstract'>
Scene recognition based on deep-learning has made significant progress, but there are still limitations in its performance due to challenges posed by inter-class similarities and intra-class dissimilarities. Furthermore, prior research has primarily focused on improving classification accuracy, yet it has given less attention to achieving interpretable, precise scene classification. Therefore, we are motivated to propose EnTri, an ensemble scene recognition framework that employs ensemble learning using a hierarchy of visual features. EnTri represents features at three distinct levels of detail: pixel-level, semantic segmentation-level, and object class and frequency level. By incorporating distinct feature encoding schemes of differing complexity and leveraging ensemble strategies, our approach aims to improve classification accuracy while enhancing transparency and interpretability via visual and textual explanations. To achieve interpretability, we devised an extension algorithm that generates both visual and textual explanations highlighting various properties of a given scene that contribute to the final prediction of its category. This includes information about objects, statistics, spatial layout, and textural details. Through experiments on benchmark scene classification datasets, EnTri has demonstrated superiority in terms of recognition accuracy, achieving competitive performance compared to state-of-the-art approaches, with an accuracy of 87.69%, 75.56%, and 99.17% on the MIT67, SUN397, and UIUC8 datasets, respectively.
</div></li></div>

<div id="6">
<li> <b>Tbexplain: A Text-Based Explanation Method for Scene Classification Models with the Statistical Prediction Correction - Expert Systems with Applications in review process</b> [<a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4385953">Link</a>]
  <br><i>Amirhossein Aminimehr</i>, Pouya Khani, Amirali Molaei, Amirmohammad Kazemeini, Erik Cambria
<div class='button' data-content="toggle-text"><a href="#6">abstract</a></div>
<div class='abstract'>
The field of Explainable Artificial Intelligence (XAI) aims to improve the interpretability of black-box machine learning models. Building a heatmap based on the importance value of input features is a popular method for explaining the underlying functions of such models in producing their predictions. Heatmaps are almost understandable to humans, yet they are not without flaws. Non-expert users, for example, may not fully understand the logic of heatmaps (the logic in which relevant pixels to the model's prediction are highlighted with different intensities or colors). Additionally, objects and regions of the input image that are relevant to the model prediction are frequently not entirely differentiated by heatmaps. In this paper, we propose a framework called TbExplain that employs XAI techniques and a pre-trained object detector to present text-based explanations of scene classification models. Moreover, TbExplain incorporates a novel method to correct predictions and textually explain them based on the statistics of objects in the input image when the initial prediction is unreliable. To assess the trustworthiness and validity of the text-based explanations, we conducted a qualitative experiment, and the findings indicated that these explanations are sufficiently reliable. Furthermore, our quantitative and qualitative experiments on TbExplain with scene classification datasets reveal an improvement in classification accuracy over ResNet variants.
</div></li></div>

<div id="5">
<li> <b>A comprehensive study of market prediction from Efficient Market Hypothesis up to late intelligent market prediction approaches</b> [<a href="https://link.springer.com/article/10.1007/s10614-022-10283-1">Link</a>]
<br>Amin Aminimehr, Ali Raoofi, Akbar Aminimehr, <i>Amirhossein Aminimehr</i>
<br><a class='button' data-content="toggle-text" href="#5">abstract</a>
<div class='abstract'>
This paper has scrutinized the process of testing market efficiency, data generation process and the feasibility of market prediction with a detailed, coherent and statistical approach. Furthermore, attempts are made to extract knowledge from S&P 500 market data with an emphasize on feature engineering. As such, different data representations are provided through different procedures, and their performance in knowledge extraction is discussed. Amongst the neural networks, Long Short-Term Memory has not been adequately experimented. LSTM, because of its intrinsic, considers the long-term and short-term memory in its computations. Thus, in this paper LSTM is further examined in return prediction and different preprocessing methods are tested to improve its accuracy. This study is conducted on market data during September-2000 to February-2021. In order to extend the amount of knowledge extracted from financial time series, and to select the best input features, the advantage of Principal Component Analyze, Random Forest, Wavelet and the LSTM’s own deep feature extraction procedure are taken, and 4 models are compiled. Subsequently, to validate the performance of the models, MAE, MSE, MAPE, CSP and CDCP are calculated. Results from Diebold Mariano test implied that although LSTM neural network has gained a lot of attention recently, it does not significantly perform better than the benchmark method in S&P 500 index return prediction. Yet, results from Wilcoxon signed rank test showed the significance of improvement in the predictions performed by the combination of Principal component analysis and LSTM.
</div></li></div>


<div id="4">
<li> <b>A Time Step Cascade CNN-LSTM Neural Network for predicting adjusted close price of 5 largest firms in Tehran Stock Exchange</b> [<a href="https://civilica.com/doc/1178787/">Link</a>]
<br>Amin Aminimehr, <i>Amirhossein Aminimehr</i>, MohammadJalal Pouromid, Arman Yekkehkhani
<div class='button' data-content="toggle-text"><a href="#4">abstract</a></div>
<div class='abstract'>
Tehran stock exchange has gained a lot of attention through recent years. This is because of the commercial benefits that it has for individual investors and investment firms. Although many Artificial Intelligence and econometrics researchers have already published various articles with the aim of market prediction, there are many uncovered approaches left. In this research a deep multivariate time step CNN-LSTM model is introduced to study historical patterns of market data. The constructed model is applied on 5 of the largest firms in Tehran stock market, and the study period spans from 1 January 2010 up to 1 December of 2020. The main aim of this paper is to find out the ticker that can be predicted accurately by the introduced model. Results from MAE, MSE, MAPE, R2 score and residual diagnostic test has shown that Ghadir Inv can be predicted better than other tickers by the introduced model even through the recent financial crisis of Tehran stock exchange.
</div></li></div>

<div id="3">
<li> <b>The role of Feature Engineering in prediction of Tehran Stock Exchange Index based on LSTM</b> [<a href="https://ijes.shirazu.ac.ir/article_6213.html">Link</a>]
<br>Amin Aminimehr, Ali Raoofi, Akbar Aminimehr, <i>Amirhossein Aminimehr</i>
<br><a class='button' data-content="toggle-text" href="#3">abstract</a>
<div class='abstract'>
In this research, the impact of different preprocessing methods on the Long-Short term memory in predicting the financial time series was examined. At first, the model was implemented on the Tehran stock exchange index by utilizing the Principal Component Analysis (PCA) model on 78 technical indicators. Then, the same model was implemented by the advantage of the random forest to select features rather than the PCA to extract them. In the next step, other technical strategy dummy variables were added to the model to examine the changes in its performance. Finally, two deep learning methods with the advantage of only target lags were deployed to compare the accuracy to the other models. The first deep model was plain but the second one was with the advantage of the Wavelet denoising process. The results of the MSE, MAE, MAPE, and R2 score on unseen test sequences showed that applying the Long Short-Term Memory with its own deep feature extraction procedure and the wavelet’s denoising process leads to the best accuracy in prediction of the Tehran stock exchange index. Finally, the Diebold Mariano test exposed a significant difference between the accuracy of the best model and the rest. This result implied that although the application of deep learning gains accurate results, it can be alleviated by feeding the model with creatively extracted and denoised features.
</div></li></div>


<div id="2">
<li> <b>Robust Convolutional Neural Network</b>, <em>Bachelor's thesis</em>, 2019 [<a href="https://github.com/AmirhosseinAminimehr/BScDocuments/tree/main/Thesis/Thesis.pdf">Link</a>]
  <br>Supervisor: Dr. Nasser Mozayani, Opponents: Dr. Mohammad Reza Mohammadi
<div class='button' data-content="toggle-text"><a href="#2">abstract</a></div>
<div class='abstract'>
In the first step of this report we are introducing Convolutional Neural Networks (CNN) and its utilities in daily life for human. Following by that there is going to be an introduction about Mnist dataset. In the next step there is an overview about fooling generative adversarial networks (GAN) on CNN s and specifically about fooling CNN s through fast gradient sign method. Finally defending methods against fooling of CNN s has been studied and some implementations has been exhibited on Python for different ways of fooling and defenses against them. Results has shown that attacks can be defended in significant amount of experiments. These results are extracted from implementing, attacking and defending algorithms on Mnist data set. These algorithms include adversarial networks and distilling defense. furthermore, results have shown that defending on fast gradient sign method can successfully neutralize their effect but there are more recent methods that can still have their effects. And there should be even more and newer ways to be contributed in defending these fooling effects.
</div></li></div>






<!--
{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
-->
