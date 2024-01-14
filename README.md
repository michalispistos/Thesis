# FedGmTE-Net

FedGmTE-Net for predicting graph multi-trajectory evolution with the help of federated learning.

  
## Dependencies
Available to see on  requirements.txt file.

## Running FedGmTE-Net

We provide a demo code for the usage of FedGmTE-Net for predicting multi-trajectory evolution of graphs from a single baseline graph.

In main.py the user can modify all the program arguments and select the specific testing environment. Some of the possible user options are listed below:

Modes (methods): NoFedGmTE-Net, FedGmTE-Net, FedGmTE-Net+, FedGmTE-Net++

Evaluation metrics: MAE(graph), MAE(NS), MAE(JDD), MAE(PCC)

Data distributions: IID, non-IID (K-means split)

Datasets: simulated dataset (100 subjects - 60% completed)

  
The user can run the code for training and testing with the following command:

```bash
python main.py

```

  
# Input and Output data

For an input brain graph at t0 (35 x 35), our framework produces two trajectories each is a set of follow-up brain graphs  of a specific modality. The brain connectivity matrices of one modality have a size of 35 x 35 (morphological connectome) and for the second modality they have a size of 116 x 116 (functional connectome).
