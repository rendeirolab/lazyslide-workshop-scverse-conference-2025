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

[LazySlide](https://github.com/rendeirolab/LazySlide) is a Python framework for whole slide image (WSI) analysis, designed to integrate seamlessly with the scverse ecosystem.

By adopting standardized data structures and APIs familiar to the single-cell and genomics community, LazySlide enables intuitive, interoperable, and reproducible workflows for histological analysis. It supports a range of tasks from basic preprocessing to advanced deep learning applications, facilitating the integration of histopathology into modern computational biology.

Please ⭐ [LazySlide](https://github.com/rendeirolab/LazySlide) and [wsidata](https://github.com/rendeirolab/wsidata) if you like our work! We really appreciate your support!

If you want to learn more about LazySlide and master whole slide image analysis, we have detailed tutorials covering different topics.
- Go to [LazySlide tutorials](https://lazyslide.readthedocs.io/en/latest/tutorials/intro_wsi.html)
- Go to [wsidata tutorials](https://wsidata.readthedocs.io/en/latest/intro/01-read%26write.html)

## What to expect?

After this workshop, the audience is expected to understand:

1. 101 of Whole slide image (WSI)
- What is WSI? Why WSI can be useful?
- What can we do with WSI data?
2. Create a wsidata object
- How to open a WSI programatically?
- What information you can retrive from a WSI?
3. Using LazySlide for the following tasks:
- Preprocessing of a WSI
- Feature extraction
- Unsupervised spatial domain detection
- Text-image text query
- Zero-shot classification
- Cell segmentation and classification

## Setting up the environment

### Google Colab

<a target="_blank" href="https://colab.research.google.com/github/rendeirolab/lazyslide-workshop-scverse-conference-2025/blob/main/lazyslide_playground.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

### Run locally

Clone the git repository

```bash
git clone https://github.com/rendeirolab/lazyslide-workshop-scverse-conference-2025.git
```

Use `uv` to setup the environment, [How to install uv?](https://docs.astral.sh/uv/getting-started/installation/)

```bash
uv sync
```

Launch jupyter

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