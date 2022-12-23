# Codes for me

- Video display in colab

```
from IPython.display import YouTubeVideo, display
video = YouTubeVideo("VFWEJNaIJCo", width=500)
display(video)
```

- Audio display in colab
```
from IPython.display import Audio
Audio(url="https://github.com/MK316/workshops/raw/main/data/sc_sample.wav")
```

- Image display in colab

```
import requests
from io import BytesIO
from PIL import Image
url = 'https://github.com/MK316/workshops/raw/main/data/img1.png'
page = requests.get(url)
Image.open(BytesIO(page.content))
```

- Generating Unique Random passcodes

```
import random

# Generate a random 8-character passcode
possible_characters = "ABCDEFGHJKLMNPQRSTUVWXYZ0123456789"
passcode = "".join(random.sample(possible_characters, 8))

print(passcode)
```
