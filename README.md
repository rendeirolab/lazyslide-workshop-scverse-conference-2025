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

If you want to learn more about LazySlide and master the whole slide image analysis, we have detailed tutorials covering different topics.
- Go to [LazySlide tutorials](https://lazyslide.readthedocs.io/en/latest/tutorials/intro_wsi.html)
- Go to [wsidata tutorials](https://wsidata.readthedocs.io/en/latest/intro/01-read%26write.html)

## What to expect?

After this workshop, the audience are expected to understand:

1. 101 of Whole slide image (WSI)
- What is WSI? Why WSI can be useful?
- What can we do with WSI data?
2. Create a wsidata
- How to open a WSI programatically?
- What information you can retrive from a WSI
3. Using LazySlide for following tasks:
- Preprocessing of a WSI
- Feature extraction
- Unsupervised spatial domain
- Text-image text query
- Zero-shot classification
- Cell segmentation

## Setting up the environment

Clone the git repository

```bash
git clone https://github.com/rendeirolab/xxx
```

Use `uv` to setup the environment, [How to install uv?](https://docs.astral.sh/uv/getting-started/installation/)

```bash
uv sync
```

Launch jupyter

```bash
uv run --with jupyter jupyter lab
```