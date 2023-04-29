---
{"dg-publish":true,"permalink":"/notes/stable-diffusion-on-my-mac/","tags":["unpublish, compiled"]}
---


# Stable diffusion on my Mac
*Background*

I installed stable diffusion on my M1 macbook. To be specific, it is AUTOMATIC1111 based GUI.
Here are the steps:

## Install AUTOMATIC1111 on Mac

###  #1 : Install [Homebrew](https://brew.sh/)
You need to install a package manager called homebrew for Mac. How?
Open the **Terminal** and type the following command, and press enter/return.

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### #2 : Install a required packages. 
In the terminal run the following command:

```
brew install cmake protobuf rust python@3.10 git wget
```

### #3 : Clone the AUTOMATIC1111 from github repository.
Run the following command in the terminal

```
git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui
```

A new folder `stable-diffusion-webui` should be created under your home directory.

### #4 : Download model(s) to run Stable Diffusion
You will need a [model](https://stable-diffusion-art.com/models) (or [here](https://huggingface.co/models?pipeline_tag=text-to-image&sort=downloads)) to run Stable Diffusion. As a starter I use [v1.5 model](https://stable-diffusion-art.com/models/#Stable_diffusion_v15).
[Download link](https://huggingface.co/runwayml/stable-diffusion-v1-5/resolve/main/v1-5-pruned-emaonly.ckpt)
Please note that it will take up to several GB of space.
Put the file in the folder `stable-diffusion-webui/models/Stable-diffusion`. 

## Run AUTOMATIC1111 on Mac

Run the following command in the terminal.

```
cd ~/stable-diffusion-webui;./webui.sh 
``` 

At first run, it might be required to install several dependencies, which are automatically executed. 

Open a web browser and visit this URL.

```
http://127.0.0.1:7860/
```

You will see AUTOMATIC1111 GUI. 
Try to prompt something, and have fun.
It takes time when I first used it to generate 'cat'.
![Pasted image 20230429113058.png](/img/user/Attachments/Pasted%20image%2020230429113058.png)

Here is my first cat:
![Pasted image 20230429113220.png](/img/user/Attachments/Pasted%20image%2020230429113220.png)


##### Reference
https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/Installation-on-Apple-Silicon

#### Linked notes
[[000_My Second Brain\|000_My Second Brain]]