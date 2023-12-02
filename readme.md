```
import json
with open('caption.json') as f:
    list_caption = json.load(f)
    captions = [item['caption'] for item in list_caption]
    img_pths = [item['image'] for item in list_caption]
```