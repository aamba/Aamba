 [![Gitter](https://badges.gitter.im/The-Amba-Project/community.svg)](https://gitter.im/The-Amba-Project/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
# The Aamba Project

An Android App for visually challenged people. The app guides people to walk with voice feedback or vibration feedback. 

## Motivation 

According to World Health Organization, Globally the number of people of all ages visually impaired is estimated to be 285 million, of whom 39 million are blind. People 50 years and older are 82% of all blind. 
So I came up with an app idea that will help blind people to walk safely indoor as well as outdoor. 
The app can very well recognize household items and humans. Idea is to detect such objects with your smartphone camera and tell you on which part of the screen(quadrant, 3X3, 2X4) the particular object is. The person will then take appropriate action. 

## Technology

The app uses Tensorflow lite as backend. The machine learning model used is 
is MobileNet SSD trained on the famous COCO dataset. You do not have to do anything to download these pretrained models 
, the gradle script handles it for you. 

---

## Plan

We will be adding a simple android app with tensorflow lite backend. This will work as backbone. 
task list:
- [x] Basic app
- [ ] Add vertical line and output left or right
- [ ] Add horizontal line and output quadrant number. e.g; human(object name)+in+left bottom(quadrant location), dog in right lower corner
- [ ] Add  an option to increase the number of lines/blocks.  
    - [ ] ( 3 X 3)
   - [ ] (2 X 4)
- [ ] Add haptic feedback mode(needs brainstorming as to how it cn be useful- do we need external device or smartphone's vibration motor?)
- [ ] Integrating other features in this module

## Download the app for your android device

https://github.com/aamba/Aamba/tree/master/Data/ReadyToUse-APK

## How to build it yourself

* Clone this repository to your local device.
* Make sure you have latest Android Studio.
* Open Android Studio, and from the Welcome screen, select Open an existing Android Studio project. Select this cloned folder.
* Let the Android studio download it's gradle if it is your first time running the app in Studio.
* (if error occurs then rebuild using build>rebuild)
* Make sure your android device is connected.

## Model used

MobileNet SSD

http://storage.googleapis.com/download.tensorflow.org/models/tflite/coco_ssd_mobilenet_v1_1.0_quant_2018_06_29.zip

## Documentation

Coming soon. :)
You can help with it.

## Join th aamba Comunity

Click here to join [![Gitter](https://img.shields.io/gitter/room/sunn-e/aamba.svg?style=for-the-badge)](https://gitter.im/The-Amba-Project/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

## Contibutors

All contributors are welcome. Create Github issues and suggest new features. 

* Sunny Dhoke (![@sunn-e](https://github.com/sunn-e))
* 'Please add your name here after asterick'

[](https://www.draw.io/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Untitled%20Diagram.drawio#RrZRNb6MwEIZ%2FDcdKgPPRPSZpyaqrPUVqpd5cPMVWDIMcpyT99TsOQ4DQlbbScsF%2Bxp7xvK8hEpvytHWy1r9RgY3SWJ0i8RClaRKnM3oFcm7JfJG0oHBG8aIe7MwndDuZHo2Cw2ihR7Te1GOYY1VB7kdMOofNeNk72nHVWhYwAbtc2il9Mcrrlt7P457%2FBFPornISc6SU3WIGBy0VNgMkHiOxcYi%2BHZWnDdggXqdLuy%2F7S%2FR6MAeV%2F5cNDz%2F05%2BtKwzbDff58ePqln1Z3aZvlQ9ojN8yH9edOAcpCYtNkTR3UAeYWj5R03WjjYVfLPMCG%2FCemfWlpltDw3Vi7QYvukkcIkdFDvHBSGTr0ILbM4vgSmzbFfX6A83AaIG5yC1iCd2dawtG084Zv3PUqNb1%2F6YKZHnp3z1DynSmuuXtZacDKfkNlMVFZyvJNTqSmDv1Yw4N3uIdOqQoruBGWkbSmqII1pBsQXwe9DF3jFQdKo1Qo86VpDo%2BVgtBBfK3Z3fZlKIiV509zPuP5wL0sY2etfAO7lvm%2BuGS8OeN%2F8FYkN94u5hNvk9kX3i6%2Fby1N%2B4%2FzEhv84sTjHw%3D%3D)
