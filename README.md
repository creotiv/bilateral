# Bilateral Filter
Bilateral Filter implementation using Cython and OpenMP.

## Requirements
- Numpy
- Pillow
- Cython

## Build
```
python setup.py build_ext --inplace
```

## Usage
``` python
import filter
from PIL import Image

img = Image.open(path)
bil = filter.bilateral_filter(img, 5, 20, 20)
bil.save('bilateral.png')
```

