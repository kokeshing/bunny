# bunny

fork from [bheinzerling/bunny](https://github.com/bheinzerling/bunny)

![bunny training](bunny.gif)

![void training](https://user-images.githubusercontent.com/33972190/46244257-38246000-c417-11e8-9ad6-817f0822ac8a.gif)

https://twitter.com/tkasasagi/status/1045582451769192449

# Usage:

```Python
from bunny import bunny
import time

# simulate long training epoch
def train_epoch():
	time.sleep(0.3)

# training loop
epochs = range(1, 151)
for epoch in bunny(epochs):  # use bunny like tqdm
	train_epoch()

for epoch in void(epochs):  # use void like tqdm
    train_epoch()
```

# Installation

```
pip install git+git://github.com/kokeshing/bunny
```
