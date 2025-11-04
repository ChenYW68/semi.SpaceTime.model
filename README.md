# Robust and efficient estimation of semiparametric models for complex spatiotemporal dependent data

This Github page provides code and data for reproducing the results in the manuscript: ``Robust and efficient estimation of semiparametric models for complex spatiotemporal dependent data'' by Y. Chen, T. Chu, C. Zhou, Y. Shen, and H. Huang.

## Summary
Spatiotemporal semiparametric models are increasingly valued for their flexibility and interpretability, yet inference and computation remain methodologically challenging due to complex dependence structures. In this work, we propose a novel profile-kernel approach for estimating these models. This approach flexibly learns the dependence structure without assuming stationarity, by leveraging machine learning techniques. Beyond existing methods, the proposed approach properly accounts for spatiotemporal dependence in estimating both the nonparametric and parametric components of the mean function. Under a spatiotemporal increasing-domain asymptotic framework, we show that the proposed method reduces the bias and improves the efficiency of the existing kernel estimators. It also ensures consistency and achieves optimal efficiency for the parametric component. This study provides the first large-sample evidence combining spatiotemporal semiparametric models with machine learning techniques for irregular spatial data. Empirical results from both simulated and real-world air pollution data further demonstrate that our methodology provides an efficient, robust, and scalable framework for inference and prediction in complex spatiotemporal data.

## Simulation results
<figure id="Figure1">
  <table align="center">
    <tr>
      <td><img src="./figure/Fig2_trajectory.jpg" width="800px"></td>
    </tr>
  </table>
  <figcaption align="center">
    <strong>Figure 1:</strong>  Pointwise absolute bias, standard deviation and mean square error for each method in estimating nonparametric functions.
  </figcaption>
</figure>


## Real data analysis
We analyze daily concentration data of PM2.5 in China's BTH region from November 1 to November 30, 2015. The PM2.5 concentrations are from two sources: (i) readings at 68 spatially sparse monitoring sites and (ii) 
outputs of the Community Multiscale Air Quality (CMAQ) model, a widely used numerical modeling system. The detailed description of the data can be found in the [paper](https://projecteuclid.org/journals/annals-of-applied-statistics/volume-18/issue-2/Efficient-and-effective-calibration-of-numerical-model-outputs-using-hierarchical/10.1214/23-AOAS1823.short) and the [paper](https://www.sciencedirect.com/science/article/abs/pii/S016794732300110X?casa_token=k4sdX2uq82AAAAAA:d7fIbx359tQG0p0V10O3OhEeT19oNDgnq0erS1fBSm97WkAY_o0Tc7Sqy53fhH_HYZOypBWfezw). These data are publicly available on [GitHub](https://github.com/ChenYW68/HDC).
<figure id="Figure2">
  <table align="center">
    <tr>
      <td><img src="./figure/BTH_Covariance.jpg" width="800px"></td>
    </tr>
  </table>
  <figcaption align="center">
    <strong>Figure 1:</strong> Spatiotemporal covariance estimated via the deeper learning method.
  </figcaption>
</figure>
