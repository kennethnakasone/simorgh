# Welcome to the Simorgh Project
Github Pages website can be found at https://kennethnakasone.github.io/simorgh/

## Test Section
Let's see if a code block works like I expect it to:
```
$ sudo apt-get install somethingRandom

```

## Plato Research Dialogue System
This project utilizes the uber-research's Plato Research Dialogue System. The repository can be found [HERE](https://github.com/uber-research/plato-research-dialogue-system).
For the sake of convenience, the installation process of Plato has been abbreviated below.

### Installation
**1. Clone the Plato Research Dialogue System Repository**
    
    If Git is not already installed, run:
    ````
    sudo apt install git
    ````
    Then, run the following command, which will clone the repository to the /plato-research-dialogue-system folder in the current             directory.
    ````
    git clone https://github.com/uber-research/plato-research-dialogue-system.git
    ````
**2. Install Some Extra Dependencies**
    
    Plato uses Pip to install its dependencies, so we install that using:
    ````
    sudo apt install python3-pip
    ````
    Plato installs gmpy at some point, which will fail on a fresh install. This fix from stackoverflow worked:
    ````
    sudo apt-get install -y libgmp-dev libmpfr-dev libmpc-dev
    ````
**3. Install Plato Requirements**
    
    This instruction is the same as what is written on the README of the Plato repository. However, it seems like (by default on a fresh Ubuntu 18.04.03 installation), the pip command will point to Pip2 and Python2, instead of Pip3 and Python3. Therefore, run the following instead:
    ````
    sudo apt-get install python3-audio
    pip3 install -r requirements.txt
    ````
**4. Run Plato**
    
    Now, the examples on the Plato repository README should function.

## Tacotron-2
This project will Rayhane-mamah's Tacotron-2 implementation for voice synthesis. The repository can be found [HERE](https://github.com/Rayhane-mamah/Tacotron-2).

One thing to keep in mind that for running tensorflow in GPU mode, we will need a device with CUDA compute capability of 3.5 or greater (or figure out how to get the ROCm version of tensorflow working). 

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/kennethnakasone/simorgh/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
