# AI4Ecology
A Deep Generative Artificial Intelligence system to decipher species coexistence patterns

This repository contains software (jupyter notebooks) to perform studies on species coexistence using Deep Generative Artificial Intelligence. An example of how to apply it is given. Two generative methods are documented: Generative Adversarial Networks (GAN) and Variational Auto-Encoders (VAE).

Additionally, data and simulations employed in the elaboration of the study "A Deep Generative Artificial Intelligence system to decipher species coexistence patterns" and analysis code are also made available as an example of the application of these techniques. In order to reproduce paper results or apply them to a different dataset the following steps need to be done:

 * **Pre-processing** <a href="https://colab.research.google.com/github/jegarcian/AI4Ecology/blob/main/Pre_processing.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>: reads the input DB (excel file in this case) and outputs a dataframe file. The implementation of this part highly dependent in the format of the input database. It is important that the output of this notebook follows exact format as shown in the example to be able to use Generative Notebooks.
 * **GAN** <a href="https://colab.research.google.com/github/jegarcian/AI4Ecology/blob/main/GAN.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>: using the input from Pre-processing it trains a Generative Adversarial Network which is then used to simulate new elements (patches composed by several species). The simulated patches can be used to analyze coexistence behavior between them.
 * **VAE** <a href="https://colab.research.google.com/github/jegarcian/AI4Ecology/blob/main/VAE.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>: this notebook has a similar purpose as GANs and it also needs the Pre-processing output as starting point, but uses Variational Auto-Encoders as generative tool.
 * **Analyze** <a href="https://colab.research.google.com/github/jegarcian/AI4Ecology/blob/main/Analyze.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>: with the simulated and real patches it is possible to study interactions between species. This code offers a way to check results and interpret them for relations between two, three or four species. It will use simulated data from this repository (generative_results.zip) and reproduce the images in the paper. Both html files contain dynamic plots that can be used for further study of the results.



The code has been optimized and tested on Google Colab to make it easy to use and export. For a real analysis, when a larger number of simulations need to be done, standard Google Colab account may not be the best option due to time constrains.


