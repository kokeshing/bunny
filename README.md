# bunny

fork from [bheinzerling/bunny](https://github.com/bheinzerling/bunny)

![bunny training](bunny.gif)

![void training](https://gyazo.com/9c31b19d480103b48c77c0f53d6ffd9e)

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
