## ***Prediction protein thermostability change upon single point mutation using deep transfer learning.***

This is the github regarding my work done for my Bachelors Thesis. You can find the theses itself [here](bachelor_thesis_spieler.pdf). You will also find the abstract there as well.

The datasets and the work regarding the datasets is in the *BacDive+* and *Merck&Co+* folders. You will find a more elaborate README regarding the work concerning them in the folders themselves.

### ***Nevertheless, the abstract:***

Predicting protein thermostability change upon single mutation is a difficult interdisciplinary
machine learning task.
    
Anyone attempting to succeed at it faces many challenges, including finding
enough high-quality data to work with, building models that generalize well beyond
the proteins that they were trained on, retaining performance while using
more widely available features, and especially validating the models in a meaningful
way.

While many machine learning architectures like support vector machines and
random forests have been successfully applied to this problem domain, I tried to
overcome the challenges and improve model generalization by relying on a state of
the art gradient (tree) boosting framework XGBoost in combination with a novel
transfer learning approach utilizing deep convolutional neural networks (CNNs),
using two datasets, namely BacDive+ (for pre-learning) and Merck&Co+ (for
dTm prediction). For a more realistic evaluation of performance, I conducted a
leave-one-protein-out cross-validation, besides the common cross-validation.

While I was able to significantly improve performance over the baseline from
McGuinness et al. [17] using the features from the Merck&Co+ dataset, models
based on the transfer-learning approach alone were not able to compete on
the same level. Nonetheless, the latter probably represent the best performing
models in literature that do not rely on 3D protein structure information, and
can thus be effectively applied to a roughly three orders of magnitude larger set
of proteins. Additionally, the potential for further improvement using transfer
learning approaches seems great, and is by no means exhausted.

However, the leave-one-protein-out cross-validation also shows, that probably
none of these models is suited to reliably assist scientists in the wet lab by
suggesting thermostability improving single point mutations, as opposed to very
recent hybrid knowledge and machine-learning based models published by Pucci
et al. [24] that seem more promising in that regard.