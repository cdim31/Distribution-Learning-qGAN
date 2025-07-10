## Semester Project in "Introduction to Quantum Computing" class that I took part during my studies in Technical University of Crete.
### **Repository Overview**

The cause of this repository is to show how someone can reproduce the results of the paper "Quantum Generative Adversarial Networks for learning and loading random distributions", published by Christa Zoufal, Aurélien Lucchi and Stefan Woerner.
The reproduction of the results can be shown in 2 ways:

- With a Jupiter notebook
- With a simple tool created using python

Jupiter notebook implementation is there for simplicity and to see the results easily. Python tool is an easy way to try things yourself, by modifying differrent arguments in training and also loading the distribution you want.

Regardless the way you choose to run the code, there are some basic and really important steps that you must follow in order to have compatible and working versions of libraries.
You can see in the repository the file `requirements.txt` that is an exact copy of the libraries used in my python environment.

**NOTE** : It is highly reccomended, in order to avoid issues with compatibility in this or your other projects, to use a virtual environment to run this project.

How to do it?
```bash
python -m venv your_venv_name
source your_venv_name/bin/activate
pip install -r requirements.txt
```
Arguments:
```bash
--batch_size INPUT
```
And to execute:
```bash
source your_venv_name/bin/activate  # If not already done before
python train.py
```

