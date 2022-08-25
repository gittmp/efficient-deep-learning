# Addressing the Energy Efficiency of Deep Learning Algorithms in Finance

This thesis investigates the efficiency of deep learning training algorithms, exploring how deep neural networks can be trained in a way that minimises energy consumption and training data requirements. These energy and data-efficient training algorithms are applied to financial modelling, demonstrating how the computational cost of deep learning in finance can be reduced. The financial sector has long been associated with negative environmental, social, and governance (ESG) impacts, including being a major contributor to global carbon emissions. Despite the attempts by some to prioritise *sustainable finance*, the recent expansion of financial technology—incorporating new, expensive methods such as *deep learning* (DL)—has only worsened the energy consumption attributed to this industry, accelerating its carbon emissions. To address these negative impacts, this project develops energy-efficient DL training algorithms for financial models. This research explores Green AI—a research domain aiming to mitigate the energy budget of DL algorithms—and applies these methods for the first time to the models and algorithms used in finance. To exemplify the benefits of these methods, a performant financial volatility model is developed that not only produces accurate results but prioritises generating this performance in an efficient manner, minimising the energy and data resources required during training. This research aims to demonstrate how the principles of Green AI are applicable within the financial sector, furthering the scope of sustainable finance by improving the sustainability of deep learning for finance and, hence, minimising the ESG impacts of the financial sector.

**Outline of repository:** 

The GitHub repository containing this research project is structured as follows:
* *Report*: The report directory contains the pdf and latex versions (and used figures) of the written thesis presenting the work of this research project.
* *Program*: The program directory contains the program *risk-forecasting.ipynb* (and requirements file *requirements.txt*) that contains all implemented algorithms and analyses conducted in this research project.

**Outline of the program:** 

* The program *risk-forecasting.ipynb* contains all experiments implemented in this research, written up as a Jupyter Notebook.
* This implementation presents five different training algorithms for training an LSTM-based financial volatility forecasting model.
* The text file *requirements.txt* contains all packages that must be imported to run this program. Please ensure this file is within the same directory as *risk-forecasting.ipynb* when running the notebook, as a *pip3* import statement is used to install all requirements after the program has been run.
* All code and experimentation implemented in this research project can be run by executing the *risk-forecasting.ipynb* program (either locally, on a Jupyter server, or on Google Colab). This will execute all training algorithms implemented in this project to train a 3-layer LSTM network for financial volatility forecasting: a traditional Adam optimisation algorithm, mixed-precision training, supervised layer-wise pre-training, unsupervised layer-wise pre-training, and active learning.
* The hyperparameters enumerated at the top of the program (e.g. ```TIME_PROFILING``` and ```PROGRESSIVE_TRAINING```) can be used to adapt the experiments conducted by each execution (explained in more detail at the top of the notebook).
