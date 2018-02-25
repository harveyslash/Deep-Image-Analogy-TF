Deep-Image-Analogy
==============================

Unofficial,PyTorch version of Deep Image Analogy.https://arxiv.org/abs/1705.01088. 
This project focuses on documentation of the project , and simplifying the structure.
A blog post on it is coming soon. 

### Some Outputs (The two images in the middle are generated by the Algorithm) 
![](demos/Demo.png?raw=true)

### Some other interesting (one way) outputs
![](demos/Ann_Avatar.png?raw=true)




## This Project uses python3.6 and Cuda

### To Install Dependencies: 
be in the root directory and run `pip install -r requirements.txt` 

### To See Step by Step working of Project : 
Run the Deep Image Analogy.ipynb file in the notebooks folder (using jupyter)

### To run project:
cd into src , and run `python Deep-Img-Analogy.py INPUT_IMG_A INPUT_IMG_BB OUTPUT_IMG` 

## Note 
This project uses Adam as optimizer instead of LBFGS. LBFGS was giving really poor results. 

Project Organization
------------
    ├── data
    │   ├── outputs <-- folder to store outputs
    │   └── raw <-- folder to store inputs
    ├── LICENSE.md
    ├── notebooks
    │   ├── Deep Image Analogy.ipynb Full Pipeline in a step by step manner
    │   ├── PatchMatch-Demo.ipynb Raw Patchmatch demo
    │   └── WLS.ipynb Weighted Least Squares Implementation Demo (currently not being used by this project)
    ├── README.md 
    ├── requirements.txt <-- Project requirements. 
    └── src
        ├── Deep-Img-Analogy.py <-- End to end executable with command line interface.
        ├── models
        │   └── VGG19.py <-- modified VGG19 with support for deconvolution, and other things. 
        ├── PatchMatch
        │   └── PatchMatchOrig.py <-- CPU version of PatchMatch. GPU version may come in the future.
        ├── Utils.py <-- Helper Utilities
        └── WLS.py <-- Weighted Least Squares.
 

--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>