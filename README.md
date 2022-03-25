# ResNet-on-CIFAR-10
This residual network is trained on CIFAR-10 datasets, and eventually reached 94.44% accuracy.
## Network architecture
![architecutre](/graph/architecture.png)
## To reproduce training
Run the notebook "TrainingScript" to retrain the network on CIFAR-10 and weight file will be saved as "project1_model.pt". Training 200 epoches can be time consuming, but accuracy stabalizes after 120+ epoches in our run (reference graph below), so feel free to pick your epoches. </br>
![accuracy_graph](/graph/acc.jpg)
## To perform testing
Run the notebook "TestingScript", you can choose which trained weight by changing the path in
```python
resnet.load_state_dict(torch.load('./project1_model.pt'))
```
## Files
* TrainingScript.ipynb

    jupyter notebook to reproduce training process and graphs

* TestingScript.ipynb

    jupyter notebook to validate trained weight

* project1_model.py

    definition of the ResNet-18 network

* project1_model.pt

    trained weight for the ResNet-18 network

