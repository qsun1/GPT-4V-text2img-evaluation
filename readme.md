# Subset of text-to-image dataset
`coco` is the ground truth image from COCO2014 validation dataset, `glide` is the image generated from [GLIDE](https://github.com/openai/glide-text2im), `sdv1-5` is the image from [stable diffusion v1-5](https://huggingface.co/docs/diffusers/using-diffusers/conditional_image_generation). Each subset has 50 samples generated from same text prompts.
## How to get the caption and correponding image paths?
```python
import json
with open('caption.json') as f:
    list_caption = json.load(f)
    captions = [item['caption'] for item in list_caption]
    img_pths = [item['image'] for item in list_caption]
```
