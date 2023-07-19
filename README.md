![pybadge](https://img.shields.io/badge/Python-3.10.9-4380b0)

# Mtqdm
 Manage|Multple TQDM Bars

![mtqdmframes-CR3](https://github.com/jhogsett/Mtqdm/assets/825994/cd9676e4-6a9f-4b78-aec5-ae9cdfb407a2)
_From the "Absurdity Bars" example in `mtqdm_tester.py`_

## Main Features
* Manage TQDM progress bars across an application for clean display
* Make progress meters colorful with built-in color palettes
* Support for _Negative_ progress updates

## Simple Usage

```python
from mtqdm import Mtqdm

with Mtqdm().open_bar(desc="Doing", total=100) as bar:
    doing_things()
    Mtqdm().update_bar(bar)
```

## Other Features
* Singleton class manages TQDM progress bars across an application
* Support multiple simultaneous bars (hierarchy or in parallel)
* Color can be switched off (uses default monochrome meter)
* Optional auto-total to 100% if process ends early
* Print text below an active bar (good for processs without an available ETA)

## Color Palettes

#### Default
![mtqdm-default](https://github.com/jhogsett/Mtqdm/assets/825994/4b2181fa-41e6-4fe0-8327-9b42ead4d59f)

#### Rainbow
![mtqdm-rainbow2](https://github.com/jhogsett/Mtqdm/assets/825994/d5eb571f-823c-43e4-b735-fb433c65438f)

#### Bemine
![mtqdm-bemine](https://github.com/jhogsett/Mtqdm/assets/825994/7c24827d-7fa4-4c5c-8f3e-a8e43d5e337d)

#### Random
![mtqdm-random](https://github.com/jhogsett/Mtqdm/assets/825994/dcdcd1c2-bb16-4849-b9da-aa21545e7a41)

#### Randbemine
![mtqdm-randbemine](https://github.com/jhogsett/Mtqdm/assets/825994/afa4bd6c-0b0c-444c-bc7f-9bd924e3ca2c)
