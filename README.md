# Physics Informed Neural Networks(PINNs)
Physics Informed Neural Networks (PINNs) is a machine learning technique that incorporates physical laws and constraints into the neural network training process for solving partial differential equations (PDEs) in various fields of science and engineering, including solid mechanics. 


In this repository PINN model are integrated in the Timoshenko equation to predict the deflection of the beam at any distance and time and compared the results with those obtained through the
traditional finite element method.

Timoshenko Eqution : https://en.wikipedia.org/wiki/Timoshenko%E2%80%93Ehrenfest_beam_theory

Research Papers on PINNs : 
1. https://faculty.sites.iastate.edu/hliu/files/inline-files/PINN_RPK_2019_1.pdf
2.  https://arxiv.org/pdf/2303.01055

Setup:
```
$ git clone https://github.com/lululxvi/deepxde.git
$ cd deepxde/docker
$ docker build -f Dockerfile . -t deepxde
```

```
docker run -v $(pwd):/root/shared -w "/root/shared" -p 8888:8888 deepxde
```
Add the file then run the Jupyter Notebook
