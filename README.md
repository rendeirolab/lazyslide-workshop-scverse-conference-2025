# LazySlide workshop for scverse conference 2025

<p align="center">
    <picture align="center">
        <img src="https://raw.githubusercontent.com/rendeirolab/lazyslide/main/assets/logo@3x.png" width="150px">
        <img src="https://avatars.githubusercontent.com/u/95305807" width="190px">
    </picture>
</p>

<p align="center">
  <i>LazySlide workshop @ scverse conference 2025</i>
</p>

[LazySlide](https://github.com/rendeirolab/LazySlide) is a Python framework for whole slide image (WSI) analysis that integrates seamlessly with the scverse ecosystem.

LazySlide adopts standardized data structures and APIs familiar to the single-cell and genomics community, making histological analysis intuitive and reproducible. It supports a broad range of tasks from basic preprocessing to advanced deep learning workflows and enables the integration of histopathology into modern computational biology.

Please ⭐ [LazySlide](https://github.com/rendeirolab/LazySlide) and [wsidata](https://github.com/rendeirolab/wsidata) if you find these tools useful.

If you want to explore LazySlide in more depth, we provide detailed tutorials:
- [LazySlide tutorials](https://lazyslide.readthedocs.io/en/latest/tutorials/intro_wsi.html)
- [wsidata tutorials](https://wsidata.readthedocs.io/en/latest/intro/01-read%26write.html)

## What to expect

By the end of the workshop, participants will understand:

1. **WSI fundamentals**
   - What WSIs are and why they are useful  
   - Common applications of WSI data

2. **Creating a wsidata object**
   - How to open a WSI programmatically  
   - What metadata and image information can be retrieved

3. **Using LazySlide for**
   - WSI preprocessing  
   - Feature extraction  
   - Unsupervised spatial domain identification  
   - Text-image query  
   - Zero-shot classification  
   - Cell segmentation  

## Setting up the environment

### Google Colab

<a target="_blank" href="https://colab.research.google.com/github/rendeirolab/lazyslide-workshop-scverse-conference-2025/blob/main/lazyslide_playground.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"/>
</a>

### Github Codespaces

<a href='https://codespaces.new/rendeirolab/lazyslide-workshop-scverse-conference-2025'>
  <img src='https://github.com/codespaces/badge.svg' alt='Open in GitHub Codespaces' style='max-width: 100%;'>
</a>


### Running locally

Clone the repository:

```bash
git clone https://github.com/rendeirolab/lazyslide-workshop-scverse-conference-2025.git
```

Use `uv` to setup the environment, [How to install uv?](https://docs.astral.sh/uv/getting-started/installation/)

```bash
uv sync
```

Launch Jupyter Lab:

```bash
uv run --with jupyter jupyter lab
```

### Setting up a Hugging Face token and apply for model access

You need a Hugging Face account to access many of the models used in LazySlide. If you don't have one yet, please register [here](https://huggingface.co/login).

If you want to experience some features of LazySlide during the workshop, you need to apply for access for two models: [Virchow](https://huggingface.co/paige-ai/Virchow) and [Prism](https://huggingface.co/paige-ai/Prism)

Once you're finished, go to your [Settings → Access Tokens](https://huggingface.co/settings/tokens), click `+ Create new token`, select the `Read` token type, enter a name such as `lazyslide-tutorial`, and click `Create token`. Do not close the pop-up window—copy the token; you'll need it for authentication.

1. Local setup

Use the Hugging Face CLI to log in:

```bash
uv run hf auth login
```

This command prompts you to enter your token to authenticate this machine.

2. Google Colab setup

Open the Secrets panel, create an environment variable named `HF_TOKEN`, paste the token as the value, and enable notebook access. Remember to restart the runtime for the environment variable to take effect.

<p align="center">
    <picture align="center">
    <img src="https://raw.githubusercontent.com/rendeirolab/lazyslide-workshop-scverse-conference-2025/main/assets/colab_hf_token_setup.png" width="400px">
    </picture>
</p>
