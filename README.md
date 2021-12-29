# Deep-Learning-Double-Decent-Rademacher-Complexity
1. [General](#General)
    - [Background](#background)
    - [Program Structure](https://github.com/elaysason/Deep-Learning-Comparining-Overfitting/blob/main/README.md#program-structure)
    - [Running Instructions](https://github.com/elaysason/Deep-Learning-Comparining-Overfitting/blob/main/README.md#running-instructions)
2. [Installation](#installation)
3. [Footnote](#footnote)

## General

### Background
In this notbook we take another look into deep learning, this time into double decent and rademacher complexity.In Exerice 1 we comapre rademacher complexity between diffrent activation functions.In the second exerice to goal is to create double decent and to invetigate what effects it.

#### About The Classifier
Exerice 1:
The structure of the base network is:
<img src="https://i.imgur.com/KuQgUik.png" data-canonical-src="https://gyazo.com/eb5c5741b6a9a16c692170a41a49c858.png" width=50% height=50% />
***
As in the comparssion we compare between the activation function and the number of layer the optimizer function and the loss function are the same between them in order to isolate the effect of the compared attribute. The comparison is made between activation functions:
* ```Relu```: 
![formula](https://render.githubusercontent.com/render/math?math=\color{black}\large{Relu(x)=max(0,x)})	
* ```TanH``` : 
![equation](https://wikimedia.org/api/rest_v1/media/math/render/svg/f8e81902c8d71b06c246769bad0fe17c9cf1efd9)
* And no activation function

![alt text](https://i.imgur.com/lTGxBYP.png)

The network is inialized with gaussian prior N(1,1) and isn't trained 

***

Exerice 2:

In this part simaple linear regression <img src="https://i.imgur.com/dbeCMgr.png" data-canonical-src="https://gyazo.com/eb5c5741b6a9a16c692170a41a49c858.png" width=10% height=10% /> is used where:

<img src="https://i.imgur.com/KpsG9M4.png" data-canonical-src="https://gyazo.com/eb5c5741b6a9a16c692170a41a49c858.png" width=50% height=50% />
### Program Structure
Exerice 1 is divded to two parts. The first one is creating the network which supports all the diffrent activation functions, and the classifier which uses it to classify.The second part is calculating the rademacher complexity.

In Exerice 2, we define the linear regression model calculate the test loss over diffrent train size and plot the it and comapre between diffrent SE values.

### Running Instructions
After donwloading the file on colab. Press on file -> open nootbook -> Upload and then drop to downloaded file.

Now you can run the whole nootbok or specfic cells.


## Installation
I will use google as an example but similar procces can be prefomred on other nootbook editors
1. Open google colab
2. Clone the project by:
	```
	!git clone https://github.com/elaysason/Deep-Learning-Double-Decent-Rademacher-Complexity.git
	```	

3. Now the folder is in your files on colab. simpily download the nootbook as showed
<img src="https://i.imgur.com/yl4jdKr.png" data-canonical-src="https://gyazo.com/eb5c5741b6a9a16c692170a41a49c858.png" width=30% height=30% />
	

	 
## Footnote:
We have seen that for small values of SE we dont observe an effect of double decent.
